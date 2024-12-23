# 
#code for downloading youtube videos
from pytubefix import YouTube
link=input("Enter a link to download: ")
yt=YouTube(link)

downloader=yt.streams.get_highest_resolution()
print("Downloading....")

downloader.download(filename="Video_Download.mp4")
print("Finished Downloading.")


import qrcode
import qrcode.constants
data="https://www.facebook.com/bishwas.ale.9"
qr=qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=40,
    border=4,
)
qr.add_data(data)
qr.make(fit=True)
img=qr.make_image(fill='black', back_color='white')
img.save("qrcode_2.0, png")
img.show()

# YT_QR
