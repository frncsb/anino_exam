# anino_exam

<h2>Unity Version:</h2>
<p>The exam project used Unity 2021.3.26f upon development.</p>

<h2>System Setup:</h2>
<h3>Main Classes and Controllers</h3>
<p>SpinButton.cs: This script is responsible for handling the spin button click event. It references the SlotMachineController script to initiate the reel-spinning process.</p>
<p>SlotMachineController.cs: This script controls the functionality of the slot machine. It handles spinning the reels, calculating scores, updating UI elements, and managing game variables.</p>

<h3>Objects:</h3>
<ul>
  <li>Image[] reelImages: An array of Image components representing each reel's symbol placeholder.</li>
  <li>Sprite[] symbols: An array of sprite symbols used as reel symbols.</li>
  <li>int score2Symbols: The score value for matching 2 symbols on a line.</li>
  <li>int score3Symbols: The score value for matching 3 symbols on a line.</li>
  <li>int score4Symbols: The score value for matching 4 symbols on a line.</li>
  <li>int score5Symbols: The score value for matching 5 symbols on a line.</li>
  <li>int totalScore: A variable to store the cumulative score.</li>
  <li>int moneyCount: A variable to store the available money count.</li>
  <li>int minBid: The minimum bid amount.</li>
  <li>TMP_Text winningsText: A TextMeshProUGUI component to display the current winnings.</li>
  <li>TMP_Text moneyText: A TextMeshProUGUI component to display the available money count.</li>
  <li>TMP_Text bidText: A TextMeshProUGUI component to display the current bid amount.</li>
</ul>

<h2>Data Sources and Editing:</h2>
<p>The data sources for the slot machine symbols and scoring combinations are defined within the code:</p>
<ul>
  <li>The array symbols[] contains the sprite symbols used as reel symbols.</li>
  <li>The array lines[][] defines the line combinations for scoring.</li>
</ul>
<p><strong>To edit the symbols or add new symbols:</strong><br>
Modify the symbols[] array by adding or replacing sprite symbols.</p>
<p><strong>To edit or add new scoring combinations:</strong><br>
Modify the lines[][] array by adding or changing the line combinations.</p>

<h2>Additional Notes:</h2>
<h3>Scalability</h3>
<p>The current implementation randomizes numbers per box.</p>
<p>The current implementation supports 20 predefined line combinations.</p>
<p>By adding new sprite symbols to the symbols[] array, the system can handle more symbols.</p>
<p>The UI elements can be enlarged or adjusted to accommodate extra features or information.</p>

<h3>Flexibility</h3>
<p>The minimum bid amount (minBid) can be adjusted according to the game requirements.</p>
<p>The scoring values (score2Symbols, score3Symbols, score4Symbols, score5Symbols) can be modified to balance the game.</p>
<p>The UI elements (winningsText, moneyText, bidText) can be restyled or customized to fit the game's theme.</p>

<h3>MVC Implementation</h3>
<p>The SlotMachineController script acts as the controller, handling game logic and managing data.</p>
<p>The reelImages array represents the view, displaying the reel symbols to the player.</p>
<p>The winningsText, moneyText, and bidText components serve as the view, presenting the game's state to the player.</p>

<h2>Future Improvements/Recommendation</h2>
<ul>
  <li>Fix inefficient combination lines and bugged scoring.</li>
  <li>Addition of scroll animations per reel.</li>
  <li>Addition of music to increase entertainment.</li>
  <li>The UI can be further improved by adding more informative elements, such as a paytable or player statistics.</li>
  <li>Creation of a better UI design.</li>
</ul>
