from PIL import Image, ImageDraw, ImageFont

# Tworzenie pustego obrazu
width, height = 400, 200
image = Image.new("RGB", (width, height), "white")
draw = ImageDraw.Draw(image)

# Tekst opisu postaci
text = "Niemiecki Oficer (Major)\n53 lata, uważny, mądry, poważny"

# Wczytanie czcionki
font = ImageFont.truetype("arial.ttf", 16)

# Rysowanie tekstu na obrazie
draw.text((20, 20), text, fill="black", font=font)

# Zapisanie obrazu do pliku
image.save("niemiecki_oficer.png")

# Wyświetlenie obrazu
image.show()
