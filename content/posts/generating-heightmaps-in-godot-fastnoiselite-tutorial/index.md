+++
authors = ["Błażej Hanzel"]
title = "Generating Heightmaps in Godot | FastNoiseLite Tutorial"
date = "2024-03-30"
categories = ["Godot Tutorials"]
url = "/generating-heightmaps-in-godot-fastnoiselite-tutorial/"
featuredImage = "cover.png"
file = "heightmap-generation-tutorial.zip"
videoLink = "https://www.youtube.com/watch?v=qaPXXduOs8s"
+++

Below you can see the differences between frequencies used to generate Perlin Noise Heightmaps. The higher the frequency, the more distant the noise appears, a bit like looking at a map from a distance. If we reduce the frequency, it will look like we took one slice from the whole and enlarged it without losing any data.

<div style="display: flex; justify-content: center;">
  <div style="display: flex; flex-wrap: wrap; gap: 10px; max-width: 100%;">
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="heightmap-generation-tutorial-height_map_2-1.jpg" target="_blank">
        <img src="heightmap-generation-tutorial-height_map_2-1.jpg" alt="freq = 0.1 heightmap" style="width: 100%; height: auto;">
      </a>
      <div>freq = 0.1 heightmap</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="heightmap-generation-tutorial-height_map_1-1.jpg" target="_blank">
        <img src="heightmap-generation-tutorial-height_map_1-1.jpg" alt="freq = 0.003 heightmap" style="width: 100%; height: auto;">
      </a>
      <div>freq = 0.003 heightmap</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="heightmap-generation-tutorial-height_map_3-1.jpg" target="_blank">
        <img src="heightmap-generation-tutorial-height_map_3-1.jpg" alt="freq = 0.0003 heightmap" style="width: 100%; height: auto;">
      </a>
      <div>freq = 0.0003 heightmap</div>
    </div>
  </div>
</div>

If you are wondering what the differences are between different types of noise, you can see them in the pictures below. They were all generated using the same seed and the same parameters.

<div style="display: flex; justify-content: center;">
  <div style="display: flex; flex-wrap: wrap; gap: 10px; max-width: 100%;">
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_cellular.jpg" target="_blank">
        <img src="noise_cellular.jpg" alt="TYPE_CELLULAR" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_CELLULAR</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_value.jpg" target="_blank">
        <img src="noise_value.jpg" alt="TYPE_VALUE" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_VALUE</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_value_cubic.jpg" target="_blank">
        <img src="noise_value_cubic.jpg" alt="TYPE_VALUE_CUBIC" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_VALUE_CUBIC</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_perlin.jpg" target="_blank">
        <img src="noise_perlin.jpg" alt="TYPE_PERLIN" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_PERLIN</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_simplex.jpg" target="_blank">
        <img src="noise_simplex.jpg" alt="TYPE_SIMPLEX" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_SIMPLEX</div>
    </div>
    <div style="text-align: center; flex: 1 1 200px; max-width: 200px;">
      <a href="noise_simplex_smooth.jpg" target="_blank">
        <img src="noise_simplex_smooth.jpg" alt="TYPE_SIMPLEX_SMOOTH" style="width: 100%; height: auto;">
      </a>
      <div>TYPE_SIMPLEX_SMOOTH</div>
    </div>
  </div>
</div>
