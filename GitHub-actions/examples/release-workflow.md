Below are some essential commands for handling `Release` in GitHub Actions:

- **Create a release**:
    ```yaml
    name: Create Release

    on:
      push:
        tags:
          - 'v*.*.*'

    jobs:
      release:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Create GitHub Release
            id: create_release
            uses: actions/create-release@v1
            env:
              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
            with:
              tag_name: ${{ github.ref }}
              release_name: Release ${{ github.ref }}
              draft: false
              prerelease: false

          - name: Upload Release Asset
            uses: actions/upload-release-asset@v1
            env:
              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
            with:
              upload_url: ${{ steps.create_release.outputs.upload_url }}
              asset_path: ./path/to/your/asset.zip
              asset_name: asset.zip
              asset_content_type: application/zip
    ```

These commands are crucial for effectively managing releases in your GitHub Actions workflows.
