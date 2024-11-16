# Images Curator by Keyword

A Python script to curate images from a directory by filtering filenames based on predefined keywords. Matching files are moved to a specified folder for easy organization.

## Features

- Automatically processes image files from the specified directory.
- Filters files based on keywords present in their filenames.
- Moves matching files to a separate folder (`Selected`).

## Requirements

- Python 3.x
- Modules: os, shutil (built-in with Python)

## How to Use

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/images-curator-by-keyword.git
   cd images-curator-by-keyword
   ```

3. Open the `main.py` file and adjust the following variables:

- `source_folder`: Set the path to the folder containing your images.
- `keywords`: Add the keywords to filter filenames.

  ```python
  keywords = ["keyword 1", "keyword 2", "keyword 3", "keyword 4", "keyword 5", "and so on"]
  ```

- `selected_folder`: The destination folder for matching files. Default is `Selected`.

4. Run the script:

   ```bash
   python main.py
   ```
## Example

If the directory structure is as follows:

```
G:\My Folder\
    image 1.jpg
    image 2.png
    image 3.jpeg
```

And your keywords are:

```python
keywords = ["image 1", "image 2"]
```

The script will move `image 1.jpg`, and `image 2.png` to `G:\My Folder\Selected`.

## Notes

- The script is case-insensitive when checking filenames.
- Only common image formats (`.png`, `.jpg`, `.jpeg`, `.gif`, `.bmp`, `.tiff`) are processed.
