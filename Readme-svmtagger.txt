#Working environment: Linux system

#Need to install SVMlight if you want to use the SVM tagger in your machine
#Insall Perl

#Download SVMTool from the github

# Open terminal (Command line interface of your computer)
#In your computer, go to the path where you have SVMTool-1.3.1/bin and SVMTool-1.3.1/lib

#Command 1

export PATH=<path to SVMTool>/SVMTool-1.3.1/bin;export PERL5LIB=<path to SVMTool>/SVMTool-1.3.1/lib

#Change the content path of config.svmt which is available in <path to SVMTool>\SVMTool-1.3.1 according to your computer installation path.  

#Command 2

SVMTlearn -V 2 config.svmt

#Copy and paste the file you want to tag 
# copy and paste the file in your model you have created.
In the command below:
	First parameter: model
	Second parameter: input file name
	Third parameter: Output file name and directory
	
#In github we have already built a model for you. You can download this model from GitHub, and give the path to the location of the model as the first parameter.

#Command 3 : Tag
SVMTagger -V 2 -S LR -T 0 model path <Input file path> Output path


For further information, please contact surangika@cse.mrt.ac.lk
