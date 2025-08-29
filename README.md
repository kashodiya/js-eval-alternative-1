# JavaScript Code Executor Demo

A web-based demo application that allows users to execute arbitrary JavaScript code using the `new Function()` constructor.

## 🚀 Features

- **Interactive Code Editor**: Large textarea for entering JavaScript code
- **Real-time Execution**: Execute JavaScript code with a single click
- **Error Handling**: Displays detailed error messages and stack traces
- **Example Code Snippets**: Pre-built examples covering various JavaScript concepts
- **Responsive Design**: Clean, modern UI that works on different screen sizes
- **Security Warning**: Clear warnings about the security implications of using `new Function()`

## 🛠️ How It Works

The demo uses JavaScript's `new Function()` constructor to dynamically create and execute functions from user-provided code strings:

```javascript
const userFunction = new Function(code);
const result = userFunction();
```

## 📋 Example Code Snippets Included

1. **Basic Math**: Simple arithmetic operations
2. **String Manipulation**: Template literals and string methods
3. **Array Operations**: Map, filter, and other array methods
4. **Object Creation**: Creating and manipulating JavaScript objects
5. **Function Definition**: Defining and calling functions (including recursion)
6. **Date and Time**: Working with Date objects
7. **JSON Operations**: JSON stringify and parsing
8. **Error Handling**: Try-catch blocks and error management

## 🚦 Getting Started

### Prerequisites
- Python 3.x (for the HTTP server)
- A modern web browser

### Running the Demo

1. **Start the server**:
   ```bash
   python3 server.py
   ```

2. **Access the demo**:
   Open your browser and navigate to `http://localhost:51796`

3. **Try the examples**:
   - Click on any example snippet to load it into the editor
   - Click "Execute Code" to run the JavaScript
   - Use Ctrl+Enter as a keyboard shortcut for execution

## ⚠️ Security Warning

**IMPORTANT**: This demo uses `new Function()` to execute arbitrary JavaScript code, which can be a significant security risk in production applications. This technique can:

- Execute malicious code
- Access global variables and functions
- Potentially compromise application security

**Use this demo only for:**
- Educational purposes
- Learning about JavaScript execution
- Prototyping and experimentation in safe environments

**Never use this pattern in production applications** without proper sandboxing and security measures.

## 🏗️ Technical Implementation

### Frontend (HTML/CSS/JavaScript)
- **HTML**: Semantic structure with accessibility considerations
- **CSS**: Modern styling with responsive design
- **JavaScript**: 
  - `new Function()` for code execution
  - Error handling and result formatting
  - Interactive example loading
  - Keyboard shortcuts (Ctrl+Enter)

### Backend (Python HTTP Server)
- **Simple HTTP Server**: Serves static files
- **CORS Headers**: Allows iframe embedding and cross-origin requests
- **Port Configuration**: Uses available ports (51796, 57017)

## 📁 File Structure

```
/workspace/
├── index.html          # Main demo application
├── server.py          # Python HTTP server
├── README.md          # This documentation
└── server.log         # Server logs
```

## 🎯 Use Cases

This demo is perfect for:
- **Learning JavaScript**: Experiment with different JavaScript features
- **Code Testing**: Quick testing of JavaScript snippets
- **Educational Purposes**: Teaching JavaScript concepts
- **Prototyping**: Rapid prototyping of JavaScript logic

## 🔧 Customization

You can easily extend this demo by:
- Adding more example code snippets
- Implementing syntax highlighting
- Adding code formatting features
- Including more advanced error handling
- Adding code saving/loading functionality

## 📝 License

This is a demo application created for educational purposes. Feel free to use and modify as needed.

---

**Remember**: Always prioritize security when working with dynamic code execution in real applications!
