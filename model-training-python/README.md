# Model Traning Python

1) Directories and files required

	├───boneage-refactor    

		├───exploration.py
		├───preprocess.py
		├───checking.py
		├───train.py
		├───predict.py
		├───main.py
		├───common.py
		├───test_unittest.py
		├───mini_dataset
		│   ├───test
		│		├───orignal test png images(required)
		│   ├───test_pre
		│		├───BLANK Directory(preprocessed images will be stored)
		│   ├───train
		│		├───orignal train png images(required)
		│   ├───train_pre
		│		├───BLANK Directory(preprocessed images will be stored)
		│   ├───valid
		│		├───orignal validation png images(required)
		│   └───valid_pre
		│		├───BLANK Directory(preprocessed images will be stored)

			├───train.csv(required)
		│   ├───valid.csv(required)
		│   └───test.csv(required)

2) Installation: Install requirements from terminal-
				 pip insall -r "requiremets.txt"

3) From the terminal- run the following code

		python main.py -i INPUT1 -c INPUT2 -t INPUT3 -v INPUT4 -p INPUT5
		eg: python main.py -i True -c True -t True -v True -p True

		INPUT1: True or False- True- if image preprocessing is required
		INPUT2: True or False- True- if images need to be checked for missing or corruption
		INPUT3: True or False- True- if model training is required
		INPUT4: True or False- True- if prediction is needed on validation images
		INPUT5: True or False- True- if prediction on test images is required

		Improtant Note- For the first time, the input Input1, Input2, Input3, Input4 must be true to generate files "mean_std_age.pkl", "model.json", and "model.h5" needed to run the prediction on validation and test images. Eg- python main.py -i True -c True -t True.

4) For help: python main.py -h

