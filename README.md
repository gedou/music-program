music-program
=============
import ddf.minim.*;
Minim minim;
AudioPlayer player_sound;


void setup()
{
    minim = new Minim(this);
    player_sound = minim.loadFile("darkness in hope.mp4");
    player_sound.play();
    player_sound.loop();
}

void stop()
{
    player_sound.close();
    minim.stop();
    super.stop();
}
