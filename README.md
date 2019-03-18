#convert pdf to png
convert -density 300 simple.pdf simple_%d.png

#create filelist with files for ocr
ls *.png > filelist

#run ocr with filelist
tesseract filelist simple

