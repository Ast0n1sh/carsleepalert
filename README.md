## File Splitter and Reassembler

This repository contains tools for splitting large files into smaller parts and reassembling them back into the original file. This is particularly useful for uploading large model files to GitHub, which has a file size limit of 25 MB.

### Why This Tool is Useful

GitHub imposes a limit on the size of files that can be uploaded to a repository. This can be problematic when dealing with large files, such as machine learning models. By splitting the file into smaller parts, it becomes possible to upload each part separately and reassemble them after downloading.

### Repository Structure

- `dataset/` : Contains all the data used for training and testing the model.
- `demonstration/` : Contains a video demonstration showcasing the model running with the GUI.
- `model/` : Contains the trained model and all related files.
- `src/` : Contains all source code, including scripts for training, testing, and the GUI implementation.
  - `File Splitter & Reassembler.py` : Script and GUI for splitting files and reassembling files.

  - `Car Sleep Alert.py` : The project source code
### How to Use Split and Reassemble. Note: Here you just need to use ressembler code to join file, ignore splitter code block

#### Splitting a File

1. **Navigate to the `src` Folder**:
   Make sure you are in the `src` folder where the `file_splitter.py` script is located.

2. **Run the Splitter Script**:
   ```sh
   python file_splitter.py
   ```
   
3. **Using the GUI**:
   - Click on "Browse" to select the file you want to split.
   - Enter the target size for each part (in MB).
   - Optionally, select a save directory. If not specified, a folder with a random name will be created on the desktop.
   - Click "Split File" to start the splitting process.

#### Reassembling Split Files

1. **Navigate to the `src` Folder**:
   Make sure you are in the `src` folder where the `file_reassembler.py` script is located.

2. **Run the Reassembler Script**:
   ```sh
   python file_reassembler.py
   ```
   
3. **Using the GUI**:
   - Click on "Browse" to select the directory containing the split parts.
   - Optionally, select a save location. If not specified, the reassembled file will be saved on the desktop with the original file name.
   - Click "Reassemble File" to start the reassembling process.

### Example Use Case

You have trained a machine learning model that results in a large `.h5` file (e.g., `animal_emotion_model.h5`). To upload this model to GitHub:

1. **Split the Model File**:
   - Use the `file_splitter.py` script to split the `animal_emotion_model.h5` file into parts smaller than 25 MB.
   - Upload the split parts to your GitHub repository.

2. **Reassemble the Model File**:
   - After cloning the repository, use the `file_reassembler.py` script to reassemble the split parts back into the original model file.
   - The reassembled model file can now be used as intended.

### Dependencies

- Python 3.x
- Tkinter (for the GUI)

### Installation

Ensure you have Python 3.x installed. You can install Tkinter via your package manager:

For Debian-based systems:
```sh
sudo apt-get install python3-tk
```

For Red Hat-based systems:
```sh
sudo yum install python3-tkinter
```

For Windows:
Tkinter is included with the standard Python installation.
