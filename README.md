Gesture Recognition
 ----------------------------------------------------------------------
Very Beginning, downloaded the data folder and randomly went through different folders to see how are the image frames. As we have to predict the hand gesture, how much images are filled with hand so that we can crop the image accordingly for training. 
After folder setup in google drive, As started with script, Scipy gave some exceptional error. The ap used in the script already depreciated. So installed 1.1.0 version to work with the same script.
In image generator, followed the script and updated as require. Added script to crop (with initial image understanding we can not crop the images a lot and focus and distance of object from camera are not same for different folder). Also added script to resize and normalize the data. By generating images using this generator, observed that images are not in sequence for a particular folder. Os.listdir not pulling the file as name/ placed. So, after reviewing different folder, sorted the list by name.
Checked the generator if it is working fine and label mapping is correct, generated some random images and labels.
For model run, collected script from different cells and created a function for reusability. Also created a function to generated Accuracy and Loss curve from each model training.
For Model, we planned to try different Cnnv3D models and Cnn2D + RNN models. Initially very first model is very small and it was just to check the network. There is detailed description for each model as given in below table.
