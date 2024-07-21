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
