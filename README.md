# epic-handsign-ml
<img alt="Preprocessing worklfow" src="preprocessing workflow.svg">
Machine learning to infer sign language letters from hand tracking data

## Files

### Notebooks:
- <a href="video-timestamp-ocr.ipynb">`video-timestamp-ocr.ipynb`</a> - Optical character recognition (OCR) of spectator camera video timestamps
- <a href="package-training-data.ipynb">`package-training-data.ipynb`</a> - Preprocess and package training data
- <a href="gesture-classification-demo.ipynb">`gesture-classification-demo.ipynb`</a> - Training data augmentation and machine learning model training

### Input data files:
- <a href="2022-03-18 17-07-41.mp4">`2022-03-18 17-07-41.mp4`</a> - Time-stamped spectator camera video recorded simultaneously with hand tracking data, needed by `video-timestamp-ocr.ipynb`
- <a href="annotation schema.yml">`annotation schema.yml`</a> - Annotation schema for <a href="https://github.com/adamrehn/VideoAnnotator">VideoAnnotator</a> and `package-training-data.ipynb`
- <a href="2022-03-18 17-07-41 annotation.json">`2022-03-18 17-07-41 annotation.json`</a> - Manual annotation data from VideoAnnotator, needed by `package-training-data.ipynb`
- <a href="2022-03-18 17-07-41 hand tracking data.csv">`2022-03-18 17-07-41 hand tracking data.csv`</a> - Time-stamped hand tracking data, needed by `package-training-data.ipynb`

### Intermediate output data files:
- <a href="2022-03-18 17-07-41 timestamps.csv">`2022-03-18 17-07-41 timestamps.csv`</a> - Video timestamp OCR result from `video-timestamp-ocr.ipynb`, needed by `package-training-data.ipynb`

### Output image files for visualization:
- <a href="frame0.png">`frame0.png`</a> - Sample video frame from `video-timestamp-ocr.ipynb`:

<img src="frame0.png">

- <a href="frame0_crop.png">`frame0_crop.png`</a> - Sample cropped video timestamp from `video-timestamp-ocr.ipynb`:

<img src="frame0_crop.png">

- <a href="training data preprocessing result.svg">`training data preprocessing result.svg`</a> - Summary of training data preprocessing from `package-training-data.ipynb`
- <a href="training data preprocessing result (edit).svg">`training data preprocessing result (edit).svg`</a> - The same, with SVG errors fixed:

<img src="training data preprocessing result (edit).svg">

### Output data files:
- <a href="2022-03-18 17-07-41 training data.csv">`2022-03-18 17-07-41 training data.csv`</a> - Preprocessed training data from `package-training-data.ipynb`

## Copyright

Copyright 2022, Häme University of Applied Sciences (HAMK), Finland

## Authors' contributions

- Tiina Ahola - Training data collection
- Gert Hattingh - Video annotation
- Wangkang Jin - Machine learning
- Toni Lavonen - Training data collection
- Olli Niemitalo (Olli.Niemitalo@hamk.fi) - Training data preprocessing
- Roman Tsypin - Video annotation planning and scema
