import cv2
import pytesseract as tess
tess.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
from PIL import Image
img = cv2.imread('image.jpg')
text = tess.image_to_string(img)
print(text) 
cv2.imshow('1st image',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
