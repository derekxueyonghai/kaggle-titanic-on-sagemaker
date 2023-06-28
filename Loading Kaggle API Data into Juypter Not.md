Loading Kaggle API Data into Juypter Notebook in AWS SageMaker

1. Go to your Kaggle account. Your profile --> Settings --> API --> Create New Token; 
2. Download a 'kaggle.json' file automatically; 
3. Set up SageMaker Studio notebook instance;
4. Open up the instance, open up a terminal window; 
5. Upload 'kaggle.json' to your local drive;
6. Use 'pwd' to verify your current working directory. All the following action will be done in your current working directory instead of root directory;
7. 
```bash
mkdir .kaggle/
mv kaggle.json .kaggle/
chmod 600 .kaggle/kaggle.json
pip install --upgrade pip
pip install kaggle
kaggle competitions list
```
It lists all competitions. 

8. 
```bash
kaggle competitions download -c titanic
conda install -y -c conda-forge unzip
unzip titanic.zip
```
9. Ready to play with the rest. 

