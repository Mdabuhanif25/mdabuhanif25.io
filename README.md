# mdabuhanif25.io
My personal site 

pip install pillow imageio

from PIL import Image, ImageDraw, ImageFont
import imageio

# Set the dimensions and background color of the GIF
width, height = 300, 100
background_color = (255, 255, 255)

# Create frames for the GIF
frames = []
for i in range(10):  # Number of frames in the GIF
    # Create a new image with the specified dimensions and background color
    img = Image.new('RGB', (width, height), background_color)
    draw = ImageDraw.Draw(img)

    # Set the font and size for the "Welcome" text
    font = ImageFont.truetype('arial.ttf', 30)

    # Calculate the position to center the text in the image
    text = "Welcome!"
    text_width, text_height = draw.textsize(text, font=font)
    x = (width - text_width) // 2
    y = (height - text_height) // 2

    # Draw the "Welcome" text on the image
    draw.text((x, y), text, font=font, fill=(0, 0, 0))

    # Append the frame to the frames list
    frames.append(img)

# Save the frames as a GIF
imageio.mimsave('welcome.gif', frames, duration=0.5)  # Change duration as needed (in seconds)
