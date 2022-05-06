# Classification of ransomware based on ensemble learning
This is the guide of the project.

Ransomware Classification
--------------------------------------------------
I: Disassembling
--------------------------------------------------
1）Disassemble all the ransomwars to get asm files
2) Make sure you have label.csv file in the source folder. It contains the label information.
  	If the dataset is asm file, this step can be skipped.

--------------------------------------------------
II: Extracting Opcodes
--------------------------------------------------
1) Run extract_opcodes.ipynb file and give location where the asm files are stored in "Ransomware"
2) Make sure you have label.csv file in the source folder. It contains the label information.
	
	It will generate a "dataset.txt" file.

--------------------------------------------------
III: Train model on dataset
--------------------------------------------------
1) open train_model.py
2) enter the location of created "dataset.txt" in Step II in the variable "data"
3) This will also create 
	i) saved model with all weights
	ii) a feature N-gram CSV file.
