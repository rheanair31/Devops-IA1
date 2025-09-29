

# DevOps IA-1 – Case Study on Please Build

## 📖 Overview

This repository demonstrates the use of **[Please Build](https://please.build/)**, a fast, open-source build automation system designed for large-scale and multi-language projects.

It is part of a DevOps case study assignment to explore and implement tools outside the typical set (Git, Jenkins, Docker, Kubernetes).
Here, Please is used as a **build and test automation tool**.

---

## ⚙️ Setup & Installation

1. Clone this repo:

   ```bash
   git clone https://github.com/rheanair31/Devops-IA1.git
   cd Devops-IA1
   ```

2. Install Please Build:

   ```bash
   curl -s https://get.please.build | bash
   source ~/.profile
   echo 'export PATH=$PATH:~/.please' >> ~/.bashrc
   source ~/.bashrc
   ```

3. Verify installation:

   ```bash
   plz --version
   ```

---

## 📂 Project Structure

```
please-demo/
│── BUILD                        # Please build definitions
│── main.py                      # Python demo script
│── test_example.py               # Unit tests
│── Please_Build_Case_Study.docx  # Case study report
│── pleasew                      # Please wrapper script
│── plugins/                     # Installed plugins
└── plz-out/                     # Build outputs (ignored in git)
```

---

## 🚀 Build & Run

```bash
plz build //:hello
plz run //:hello
```

✅ Output:

```
Hello from Please Build!
```

---

## 🧪 Running Tests

```bash
plz test //...
```

✅ Output:

```
2 tests run; 2 passed
```

---

## 🔍 Comparison with Other Tools

| Feature          | Please Build  | Bazel        | Gradle        |
| ---------------- | ------------- | ------------ | ------------- |
| Language Support | Multi-lang    | Multi-lang   | JVM + plugins |
| Performance      | Very fast     | Fast         | Moderate      |
| Setup            | Single binary | Config heavy | Requires JVM  |
| Monorepo Support | ✅ Yes         | ✅ Yes        | ⚠️ Limited    |

---

## 📜 References

* [Please Build Docs](https://please.build/)
* [Please GitHub](https://github.com/thought-machine/please)

---

