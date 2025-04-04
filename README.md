# WebLLM Chat Demo

A browser-based chat application running Llama 3.2 1B directly in your web browser using WebGPU technology. This application demonstrates the capabilities of Machine Learning Compilation (MLC) for client-side AI inference.

## Features

- 🚀 Runs completely in the browser - no server required
- 💻 Uses WebGPU for hardware acceleration
- 🤖 Powered by Llama 3.2 1B model
- ⚡ Real-time streaming responses
- 📊 Performance statistics tracking
- 🎨 Clean, responsive UI with Tailwind CSS

## Requirements

- **Browser**: Chrome or Edge with WebGPU support enabled
- **Hardware**: GPU with shader-f16 feature support
- **Memory**: Minimum 2GB VRAM recommended
- **Internet**: Good connection for initial model download

## Getting Started

1. Clone this repository:
```bash
git clone https://github.com/yourusername/webllm-chat-demo.git
cd webllm-chat-demo
```

2. Serve the files using a local web server. For example, using Python:
```bash
# Python 3.x
python -m http.server 8000
```

3. Open your browser and navigate to:
```
http://localhost:8000
```

## Usage

1. Click "Initialize Model" to start loading the Llama 3.2 1B model
2. Wait for the model to download and initialize (may take several minutes)
3. Once loaded, type your message in the chat input
4. Press Enter or click the send button to get a response
5. Use the "Reset" button to clear the chat and reload the model if needed

## Technical Details

- **Model**: Llama 3.2 1B Instruct (4-bit quantized)
- **Framework**: MLC (Machine Learning Compilation)
- **UI Framework**: Tailwind CSS
- **Dependencies**:
  - @mlc-ai/web-llm
  - Tailwind CSS
  - Font Awesome

## Performance Considerations

- Initial model download size: ~879MB
- Context window size: 4096 tokens
- Low resource mode enabled for better compatibility
- Streaming responses for better user experience

## Troubleshooting

- **WebGPU Not Available**: Ensure you're using Chrome/Edge with WebGPU enabled
- **Loading Fails**: Try clearing browser cache and reloading
- **Performance Issues**: Check GPU compatibility and available VRAM
- **Cache Errors**: Disable cache in the application settings

## Privacy

All processing happens locally in your browser. No data is sent to external servers during chat interactions.

## Credits

- Powered by [MLC](https://mlc.ai/)
- Model hosted on [Hugging Face](https://huggingface.co/mlc-ai)
- UI components from [Tailwind CSS](https://tailwindcss.com/)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
