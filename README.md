# surimport pygame

# Initialize pygame
pygame.init()

# Load the sound file
sound_file = "path/to/your/sound_file.wav"
pygame.mixer.music.load(sound_file)

# Play the sound file
pygame.mixer.music.play()

# Wait for the sound to finish playing
while pygame.mixer.music.get_busy():
    pygame.time.Clock().tick(10)

# Quit pygame
pygame.quit()
