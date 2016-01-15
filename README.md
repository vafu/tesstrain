# About
Simple tesseract training script made for easy traineddata creation.
No box editing needed!

# Requirements
- imagemagick
- tesseract-3.04

# HOWTO
Pass all needed arguments to the script: training content file, language, unicharset (Latin unicharset could be found in this repo, more 
[here](https://github.com/tesseract-ocr/langdata)), and a directory with *.ttf fonts.
Run the script passing font name(s);

Example `tesstrain -l lang_extra -f ./content -u .unicharset 'Monotype Corsiva Regular' 'American Captain'`

# USAGE
USAGE:                                                                                                                                                        
     *  tesstrain [-f contentfile] [-f fontdir] [-u unicharset] [-l lang] fontname1 [fontname2 ...]                                                               
OPTIONS:                                                                                                                                                      
     * -h show this help message                                                                                                                               
     * -f provides directory with *.ttf fonts. Default is .fonts/                                                                                              
     * -u provides the unicharset file used to generate shapes. Default is .unicharset                                                                         
     * -c provides the text file used to generate tif/box pair. Default is .content                                                                            
     * -l provides the output package name. Default is engCreated by tuule_
