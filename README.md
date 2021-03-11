# download-sdl2-image

This is an action for downloading SDL2_image sources and runtime binaries on Windows using MSVC.

The downloaded headers will be stored under `sources_destination`, in a separate `SDL2_image-devel-X.Y.Z-VC` folder, where `X.Y.Z` corresponds to the `version` parameter, e.g. `2.0.14`. The `binaries_destination` is the folder where all of the runtime binaries (`.dll` files) will be stored.

Note, you will have to make sure that the destination folders exist before invoking the action.

## Usage

```yml
- name: Download SDL2_image
  uses: albin-johansson/download-sdl2-image@v1
  with:
    version: 2.0.5
    sources_destination: .
    binaries_destination: bin
```
