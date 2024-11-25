from rembg import remove
from io import BytesIO

# Remove background using rembg
with open(image_path, "rb") as img_file:
    input_image = img_file.read()

output_image = remove(input_image)

# Save the edited image with the background removed
output_path = "/mnt/data/edited_no_background.png"
with open(output_path, "wb") as out_file:
    out_file.write(output_image)

output_path

