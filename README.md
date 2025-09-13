# 📚 Simple Flashcard App

A clean, easy-to-use web application that converts your text files into interactive flashcards for studying.

## ✨ Features

- **File Upload Support**: Works with `.txt`, `.docx`, and `.doc` files
- **Auto-Parsing**: Automatically converts "Word: Definition" format into flashcards
- **Interactive Cards**: Click to flip between word and definition
- **Navigation Controls**: Previous/Next buttons and keyboard shortcuts
- **Shuffle Mode**: Randomize card order for better learning
- **Mobile Friendly**: Responsive design that works on all devices
- **No Installation Required**: Pure HTML/CSS/JavaScript - just open and use!

## 🚀 How to Run Locally

### Method 1: Direct File Opening (Simplest)
1. Save the code as `flashcards.html`
2. Double-click the file to open in your browser  
3. Start uploading files and studying!

### Method 2: If File Uploads Don't Work
Some browsers restrict file access from `file://` URLs. Use a local server:

**With Python (Recommended):**
```bash
# Navigate to the folder containing your HTML file
cd /path/to/your/flashcards/folder

# Start a local server
python -m http.server 8000

# Open your browser and go to:
# http://localhost:8000
```

**With Node.js:**
```bash
npx http-server
```

**With VS Code:**
- Install the "Live Server" extension
- Right-click your HTML file → "Open with Live Server"

## 📝 How to Prepare Your Study Files

Create a text file where each line follows this format:
```
Word: Definition
```

### Example File Content:
```
Hello: used when meeting or greeting someone
Goodbye: used when parting or at the end of a conversation
Thank you: an expression of gratitude
Please: used to make a polite request
Sorry: used to express regret or apology
```

### Supported File Types:
- **`.txt`** - Plain text files
- **`.docx`** - Microsoft Word documents
- **`.doc`** - Legacy Word documents

## 🎮 How to Use the App

1. **Upload File**: Click "Choose File" and select your study file
2. **Navigate Cards**: 
   - Click the card to flip between word and definition
   - Use "Previous" and "Next" buttons to move between cards
   - Or use keyboard shortcuts (see below)
3. **Study Features**:
   - Click "Shuffle" to randomize card order
   - Click "New File" to upload a different study set

## ⌨️ Keyboard Shortcuts

- **Spacebar** or **Enter**: Flip current card
- **Left Arrow**: Go to previous card  
- **Right Arrow**: Go to next card

## 📱 Mobile Usage

The app is fully responsive! On mobile devices:
- Tap cards to flip them
- Use the on-screen buttons for navigation
- Swipe gestures are not implemented, but buttons work great

## 🔧 Troubleshooting

**File won't upload when opening HTML directly?**
- Use Method 2 (local server) instead
- This happens due to browser security restrictions

**Cards not parsing correctly?**
- Make sure each line follows exactly: `Word: Definition`
- Check for extra spaces or special characters
- Ensure there's a colon (`:`) separating word and definition

**No cards showing up?**
- Verify your file format matches the example above
- Make sure there are no empty lines at the beginning
- Check that definitions aren't empty after the colon

## 🎯 Tips for Effective Studying

1. **Keep definitions concise** - shorter definitions are easier to remember
2. **Use the shuffle feature** - helps prevent memorizing order instead of content
3. **Review regularly** - spaced repetition is key to retention
4. **Create themed sets** - separate files for different subjects or topics

## 💡 Advanced Usage

**Multiple Study Sets**: Create different files for different subjects:
- `spanish_vocabulary.txt`
- `biology_terms.txt` 
- `history_dates.txt`

**Collaborative Study**: Share your text files with classmates - they can use the same app!

## 🛠️ Technical Details

- **No data storage**: All processing happens in your browser
- **Privacy-friendly**: Files are processed locally, never uploaded to any server
- **Lightweight**: No dependencies except for .docx file reading
- **Cross-platform**: Works on Windows, Mac, Linux, mobile devices

---

*Happy studying! 🎓*
