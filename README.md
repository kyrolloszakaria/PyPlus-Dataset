# PyPlus Dataset

## Introduction
Welcome to the PyPlus dataset repository! The PyPlus dataset is a collection of more than 250,000 pairs of natural language prompts and their corresponding commented code snippets. It has been specifically tailored to serve the ConcodePlus task in the CodeT5 model.

## Dataset Details
Here is a sample from the PyPlus dataset:

```json
{
  "code": "def load_file(self, file_path, share_name, directory_name, file_name, **kwargs):\n        \"\"\"\n        Upload a file to Azure File Share.\n\n        :param file_path: Path to the file to load.\n        :type file_path: str\n        :param share_name: Name of the share.\n        :type share_name: str\n        :param directory_name: Name of the directory.\n        :type directory_name: str\n        :param file_name: Name of the file.\n        :type file_name: str\n        :param kwargs: Optional keyword arguments that\n            `FileService.create_file_from_path()` takes.\n        :type kwargs: object\n        \"\"\"\n        self.connection.create_file_from_path(share_name, directory_name,\n                                              file_name, file_path, **kwargs)"
  "docstring": "Upload a file to Azure File Share."
}
```
This sample demonstrates a code snippet that defines a load_file function in Python. The corresponding natural language prompt describes the functionality of the code, which is to upload a file to an Azure File Share.

The PyPlus dataset consists of pairs of natural language prompts and commented code snippets. Each pair is designed to capture the mapping between a human-readable prompt and its corresponding code implementation.
The datasets contains only Python codes. As you can guess from the name ;) 
Here are some key details about the PyPlus dataset:

- **Size**: The dataset contains more than 250,000 pairs of prompts and code snippets. And it is 282MB total
- **Language**: The dataset is solely focused on the Python programming language.
- **Commented Code**: Each code snippet is accompanied by comments that explain its functionality and purpose.
- **Training and Evaluation Sets**: The dataset is split into three: training, evaluation,and test subsets. Note you can find the training split [here](https://drive.google.com/file/d/1mO6tW1Q_Xx6uV0dFh8Vzs1TuvnqDaIjF/view?usp=share_link) as it was too large to be uploaded here.

## Usage
To use the PyPlus dataset in your research or projects, follow these steps:

1. **Clone the Repository**: Begin by cloning this repository to your local machine using the Git command:
git clone https://github.com/kyrolloszakaria/PyPlus.git

2. **Explore the Dataset**: Take some time to explore the dataset and familiarize yourself with its structure and contents. You can access the natural language prompts and their corresponding commented code snippets.

3. **Preprocessing**: Depending on your specific requirements, you may need to preprocess the dataset before using it in your models. You can apply various text cleaning, tokenization, or normalization techniques as necessary.

4. **Model Training**: Utilize the PyPlus dataset for training your models. You can use it to develop models that can generate code from natural language prompts or to evaluate the performance of existing code generation models.

5. **Model Evaluation**: The PyPlus dataset also serves for evaluation and test purposes. You can assess the quality and accuracy of your code generation models by comparing their output with the annotated code snippets in the dataset.



## Contribution
We welcome contributions to the PyPlus dataset repository. If you have additional annotated code snippets or improvements to the existing dataset, feel free to submit a pull request. Please follow the guidelines mentioned in the CONTRIBUTING.md file for contributing to this repository.

## Contact
If you have any questions, suggestions, or feedback regarding the PyPlus dataset, please don't hesitate to contact us.
You can reach out via: kyrolloszakaria@aucegypt.edu 
