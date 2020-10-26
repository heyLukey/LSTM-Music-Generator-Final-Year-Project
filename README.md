
Recreating the Dataset
*********************************************************************************************************
	This folder contains all the code needed for the music generation system designed by my project.
	However, in order to fit Moodles size limit the dataset and any serialised data has been removed.

	The dataset can be recreated by downloading the MIDI files at: http://www.piano-midi.de/chopin.htm
	and placing the files in the "Dataset" folder.
*********************************************************************************************************

Directory Handling
*********************************************************************************************************
	For some functions entire directory paths must be used.
	These paths can be easily identified as they constitute the parameters for:
	ss1_model_creation and ss2_ generation
	Please change these directories to match that of the system you are using.

	The code also requires the (empty) folders given in order to write and read data to. 
	These folders are as follows:

	1. Dataset - used for storing the dataset to be used
	2. Generated_Audio - used for storing audio rendered from midi files in Generated_MIDI
	3. Generated_MIDI - used to store generated MIDI files
	4. Model_Data - used to store data relevant to model training 
	5. Pickled_Data - used to store important data structures

	A soundfont file is also provided to facilite audio rendering.
*********************************************************************************************************

Dependencies
*********************************************************************************************************
	Noteable libraries used in this code are as follows:
	1. tensorflow-gpu (2.1.0)
	2. keras (2.3.1)
	3. music21 (5.7.2)
	4. scikit-learn (0.22.2)

	This code also relies on fluidsynth (2.1.2) for the midi2wav function.
*********************************************************************************************************

Recreating Survey Music
*********************************************************************************************************
	The MIDI files used for in the project's survey can be located in Survey_music,
	Where the human pieces are in "Human" and the computer pieces are in "Computer"

	These can be rendered using midi2wav with soundfont.sf2 to recreate the audio used in the survey.
*********************************************************************************************************