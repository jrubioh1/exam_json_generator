# 📄 Exam JSON Generator (Preproduction)

**Exam JSON Generator** is a tool that converts `.DOCX` documents into `.JSON` files, provided they follow a specific predefined structure.

---

## 📐 Input Format

The `.docx` document must follow the format shown in:

```
exam_json_generator/ejemplo_formato_valido.docx
```

You can preview the structure using:
```bash
poetry run exam_json_generator --show-example
```

> ⚠️ It is **very important** to preserve:
> - Line breaks
> - Spaces
> - Accents
> - Exact position of the labels

Any deviation might result in incorrect interpretation.

---

## 🚀 How to Run

1. Enter the Poetry virtual environment:
```bash
poetry shell
```

2. Run the generator with:
```bash
poetry run exam_json_generator <input_folder> <output_folder>
```

Example:
```bash
poetry run exam_json_generator exam_json_generator/assets exam_json_generator/output
```

---

## 📂 Expected Structure

- **Input:** folder containing the `.docx` files (passed as first argument).
- **Output:** folder where the resulting `.json` files will be saved (second argument).

Both paths must be passed as arguments.

---

## ✅ Requirements

- Input files in `.docx` format
- Python 3.10+
- [Poetry](https://python-poetry.org/docs/) installed

---

## 🧪 Automatic Validation

- The program validates if the input and output folders exist.
- If the output folder doesn't exist, it will be created automatically.

---

## ⚠️ Production mode

You may alternatively install it via PYPi using:

```
pip install exam_json_generator
```
