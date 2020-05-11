## Testing Directions

Included here:

- a script for converting images to base64 and saving that in a `.txt` file - `test.py`
- 4 test images of short handwritten sentences
- 4 `.txt` files that were generated by `test.py`
- a `.json` template for creating more test files if needed
- 4 `.json` test files including the base64 from the `.txt` files

To run the tests navigate to the root `story-squad-ds` folder:

1. Change the image name in `test.py` to `<image_name>.jpg`
2. Change the `.txt` file to `<image_name>.txt` (this is just for ease of naming and navigation)
3. Open newly created `.txt` file
4. Open `text_pic_X.json`, create new file, copy contents in and rename `<image_name>.json`
5. Copy-paste base64 text from `<image_name>.txt` into appropriate place in `<image_name>.json`
6. `cd ..` into `story-squad-ds` root folder
7. run this line of code in command line
`pipenv run python dotPy/transcription.py < testing/<image_name>.json`

```python
pipenv run python dotPy/transcription.py < testing/test_pic_1.json
```