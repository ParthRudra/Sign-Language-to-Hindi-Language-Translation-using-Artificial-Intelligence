# Sign-Language-to-Hindi-Language-Translation-using-Artificial-Intelligence
This is a demo on Sign Language to Hindi Language Translation using Artificial Intelligence in Real Time.
This is an academic project with the aim of establishing fluent conversation for people who use sign language frequently.
The technical inspiration for this project comes from the work of nicholas renotte which is based on American Sign Language whereas this project is more focussed on Indian sign language translation.
There are very few datasets that are available which work on Indian sign language translation to Hindi so to begin with the project the first step was to convert Indian sign language to English and then translate from English to Hindi.
The work primarily focusses on dataset creation for five classess based on Indian sign language (Alright, Good, Hello, Thanks, You) followed by labelling of the images created using labelImg.
The images with their respective labels are split into training and testing datasets for further use to train the model.
After the images are configured the paths are setup with their respective directories to use further throughout the program.
Label map and its Annotation path is configured where a .txt file is generated and stored in that respective directory.
Further TF records are created for the tensorflow to work with the images and split into test and train records.
The my_ssd_mobnet model is used for transfer learning and object detection api to detect in real time.
Further the model was loaded for training and the best number of training steps for the model training is 10,000 steps.
The model thus trained was picked up from the checkpoint and ready to detect in real time.
The model can detect 5 classes belonging to Indian sign language in Real Time.
