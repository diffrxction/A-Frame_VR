# Solar System (Part II)

   The planetary system that we call home is located in an outer spiral arm of the Milky Way galaxy.

## Solar

   Our solar system consists of our star, the Sun, and everything bound to it by gravity — the planets Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus and Neptune, dwarf planets such as Pluto, dozens of moons and millions of asteroids, comets, and meteoroids.

   But what would your solar system look like?

   In this project, we will add textures, sky, texts, animations, and more in index.html.

   Note: This is part 2 of a cumulative project in three parts. In parts 2 & 3, we will add textures and animations to the solar system.

  - Part I. Creating the solar system.
  - Part II: Polishing.
  - Part III: Add interactions.

## Grabbing the code:

1. Because this is a cumulative project, we are going to grab the code from Solar System (Part I).
   Make sure to copy and paste the code in here.

## Adding textures to the planets:

2. Let’s add some image textures for our planets!

   Add an <a-assets> element in <a-scene> to use A-Frame’s asset management system.

3. Here are some of the skins that we made for you. They should already be your folder:

    sun.jpg
    mercury.jpg
    venus.jpg
    earth.jpg
    mars.jpg
    jupiter.jpg
    uranus.jpg
    neptune.jpg

   Feel free to use these or find other texture images on Google.

   Add them to the asset management system.

4. Now we have all the textures in the asset management system, let’s use them for your planets!
   Delete the color component of each of your <a-sphere> planets and add a src of the image texture id. Remember to add the # before the id name.

## Extra touches:

5. Add an <a-sky> with the following image or one of your choosing:

    space.jpg

6. Add one or more light sources with <a-light>.

7. Add the name of each planet using <a-text>. Or a story about the solar system.

8. The outer space is a vacuum, but for our solar system, there’s sound!
   Find a sound clip online and add it to your solar system.

## Animations:

9. Almost all of the planets in our solar system rotate in a counter-clockwise motion. The two anomalies in question are Venus and Uranus. These planets rotate in the clockwise or retrograde direction.

   Use the animation component to add some rotational animation.

   Fun fact: A single day on Venus is longer than an Earth year! It takes 243 Earth days to complete a Venus rotation (but it only takes 224.7 days to complete each orbit).
