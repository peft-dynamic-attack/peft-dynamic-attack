### Hi
# The will be a blog post

<div>
  <h3>Interactive Degree Slider</h3>
  
  <label for="degree-slider">Adjust the angle (0-360):</label>
  
  <input type="range" id="degree-slider" min="0" max="360" value="90">
  
  <p>The current value is: <strong><span id="slider-value">90</span>°</strong></p>
</div>

<script>
  // Get the slider and the output display
  const slider = document.getElementById('degree-slider');
  const output = document.getElementById('slider-value');

  // Add an "event listener" that fires every time the slider moves
  slider.oninput = function() {
    // Update the output's text to match the slider's current value
    output.innerHTML = this.value;
  }
</script>
