# My OpenAI Image Generator

This is a simple command-line application that uses the OpenAI API to generate images based on a given prompt.

## Installation

1. Clone this repository.
2. Install the required dependencies by running `pip install -r requirements.txt`.

## Usage

1. Run the application by executing `python imagey.py` followed by the necessary arguments.
2. The generated image will be saved in the `images/` directory.

The application accepts the following arguments:

- `prompt`: The prompt for image generation.
- `name`: The name of the generated image.
- `--model`: The model to use for image generation. Default is 'dall-e-3'.
- `--size`: The size of the generated image. Default is '1024x1024'.
- `--quality`: The quality of the generated image. Default is 'standard'.
- `--n`: The number of images to generate. Default is 1.

Example usage:

```bash
python imagey.py "A painting of a glass of water on a table." "water_painting" --model "dall-e-3" --size "1024x1024" --quality "standard" --n 1
```

**Note**

Make sure to set your OpenAI API key in your environment variables before running the application.

**Setting the OpenAI API Key**

Before running the application, you need to set your OpenAI API key as an environment variable. Here's how you can do this:

For Bash and ZSH shells:

1. Open your shell profile file (`.bashrc`, `.bash_profile`, or `.zshrc`) in a text editor.
2. Add the following line to the file, replacing `your_api_key` with your actual OpenAI API key:

```bash
export OPENAI_API_KEY="your_api_key"
```

3. Save the file and restart your shell.