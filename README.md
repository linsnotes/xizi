# Stroke by Stroke: Chinese Character Writer

This webpage demonstrates how to animate and practice writing Chinese characters using [HanziWriter](https://github.com/chanind/hanzi-writer). Users can enter Chinese text, animate each character’s stroke order, quiz themselves, or prepare a printable layout of the characters.

## Features

1. **Character Input**:  
   - Enter or paste Chinese text in the input box.  
   - Special placeholders:
     - **`b`**: Inserts an empty box (no character).
     - **`k`**: Forces a new line in the grid.
   - The code automatically filters out non-Chinese characters (except `b` and `k`).

2. **Grid Display**:  
   - Displays each character (or empty box) in a responsive grid.  
   - Automatically adjusts columns based on screen size.

3. **Animation Controls**:  
   - **Start / Previous**: Begins animating from the first character or moves back one character.  
   - **Next**: Moves forward to the next character and animates it.  
   - **Stop / Resume**: Pauses and resumes the current character’s animation.  
   - **Animate All**: Sequentially animates all characters. Also allows you to stop and revert at any time.  

4. **Quiz Mode**:  
   - Lets you practice writing characters stroke by stroke.  
   - Logs mistakes and completions in the message area.

5. **Print Mode**:  
   - Hides extra page elements, leaving just the character grid for easy printing.

6. **Visitor Counter**:  
   - Tracks page views using [GoatCounter](https://www.goatcounter.com).

## How to Use

1. **Open the Page**:  
   Simply open the HTML file in your browser or deploy it to a web server.

2. **Enter Chinese Text**:  
   - Type or paste Chinese characters in the input box.  
   - Optionally use `b` for empty boxes or `k` for new lines.

3. **Animate / Practice**:  
   - Click **Start** to animate from the first character (use **Previous** / **Next** to navigate).  
   - Toggle **Stop** / **Resume** as needed.  
   - Use **Animate All** to watch all characters in sequence.

4. **Quiz Yourself**:  
   - Click **Quiz Mode** to practice drawing each character.  
   - The message log at the bottom displays mistakes and completions.

5. **Print Layout**:  
   - Click **Print Mode** to switch to a simplified view for printing.

## Project Structure

- **HTML**: The entire page is contained in a single HTML file. The `<script>` at the bottom initializes HanziWriter instances and implements the logic for animation, quiz, and print mode.
- **Inline CSS**: The `<style>` block at the top handles layout, responsive grids, and basic styling.
- **Dependencies**:
  - [HanziWriter](https://cdn.jsdelivr.net/npm/hanzi-writer@3.5/dist/hanzi-writer.min.js)  
  - [GoatCounter analytics script](//gc.zgo.at/count.js)

## Customization

- **Styling**: Adjust the `body`, `.navbar`, or `.character-grid` CSS to change the layout or color scheme.
- **Animation Settings**: Modify stroke animation speed or colors in the `HanziWriter.create()` options.
- **Input Handling**: The `removePunctuationAndSpaces()` function can be customized to include or exclude specific characters.

## License

Feel free to use or modify this code for personal or educational purposes. Refer to the original [HanziWriter repository](https://github.com/chanind/hanzi-writer) for its license terms.

---

Enjoy exploring Chinese characters stroke by stroke!
