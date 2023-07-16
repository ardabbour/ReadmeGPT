# ReadmeGPT

ReadmeGPT is a toy project that uses ChatGPT to create README files for software projects.

## Prerequisites

- Python3.8+
- An OpenAI API key

## Usage

1. Get ReadmeGPT:

```bash
git clone https://github.com/ardabbour/ReadmeGPT.git
```

2. Clone the project you want to generate a README of to a folder called "project":

```bash
cd $PATH_TO_READMEGPT
git clone $MY_PROJECT_GIT_ADDRESS $PATH_TO_READMEGPT/project
```

3. Edit the constants in `main.py`
   > - Pay attention to the `ALLOW_LIST` constant. Only files (or file extentions) defined in it will be considered by ReadmeGPT.
   > - Make sure you use an appropriate model to do the job.

4. Run ReadmeGPT:

```bash
./main.py # or python3 main.py
```

The above code snippets will read the contents of the project, and prompt a GPT model to create a README for it. Both the prompt and the model's response will be saved to disk.

The README generated is almost never 100% ready for usage, but is a fantastic starting point.

### Further Usage

You can modify the `preprompt.md` file to your liking if you want to adapt to a different template.

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](LICENSE)
