# 🦫 Learn Go the Hard Way — For DevOps Engineers

> “Type it. Break it. Fix it. Repeat.”  
> Inspired by *Learn Python the Hard Way* — rebuilt for Go and modern DevOps.

---

## 📖 About

This book teaches Go the same way Zed Shaw taught Python:  
by **typing real code**, **running it**, **breaking it**, and **learning from your own errors**.  
Every exercise builds on the previous one, ending with real DevOps-grade tools you can deploy in AWS, Docker, or Kubernetes.

You’ll write **50 hands-on programs**, each small enough to understand, yet powerful enough to reuse at work.

---

## 🧰 Prerequisites
* Go 1.22+ installed (`go version`)
* Linux or macOS terminal
* Basic shell and Git knowledge
* Optional AWS/Docker/Kubernetes access for Part 4

---

## 🗂️ Project Layout

```
learn-go-the-hard-way/
    ├── README.md
    ├── part1_basics/
    │   ├── ex01_hello.go
    │   ├── ex02_comments.go
    │   └── ...
    ├── part2_functions/
    │   ├── ex11_functions.go
    │   └── ...
    ├── part3_realworld/
    │   └── ...
    └── part4_devops/
    └── ...
```

Run any example:

```bash
go run part1_basics/ex01_hello.go
````

---

## 📚 Table of Contents

### **Part 1 — Go Fundamentals**

|  #  | Exercise                | Topic                     |
| :-: | ----------------------- | ------------------------- |
|  0  | Installing Go and Setup | environment, workspace    |
|  1  | Hello Go                | your first program        |
|  2  | Comments and Printing   | `fmt.Println`, formatting |
|  3  | Variables and Constants | `var`, `:=`, `const`      |
|  4  | Numbers and Math        | ints vs floats            |
|  5  | Strings and Formatting  | concatenation, `Printf`   |
|  6  | Reading User Input      | `fmt.Scanln`, `bufio`     |
|  7  | Arrays and Slices       | `append`, `len`, `cap`    |
|  8  | Maps                    | key/value storage         |
|  9  | Conditionals            | `if`, `else`, `switch`    |
|  10 | Loops                   | `for`, `range`, `break`   |

### **Part 2 — Functions, Structs & Interfaces**

11 – 21 → functions, errors, structs, methods, pointers, packages, interfaces, time, switch/enums.

### **Part 3 — Real-World Go**

22 – 31 → CLI args, file I/O, JSON/YAML, HTTP client/server, goroutines, channels, mutexes, context.

### **Part 4 — Go for DevOps Engineers**

32 – 50 → flag-based CLI, env vars, shell automation, AWS SDK, Docker, Kubernetes, GitOps, health checks, log parsers, metrics exporters, systemd-style watchdog, AWS cost alerts, webhooks, S3 uploaders, secret vault, log forwarder, and final DevOps toolkit project.

---

## 🧱 Exercise Template

Every lesson follows this pattern:

### **Exercise N – Title**

**Goal:** *short description of what you’ll learn.*

#### Code

```go
package main

import "fmt"

func main() {
    fmt.Println("example output")
}
```

#### Run

```bash
go run exNN_name.go
```

#### Output

```
example output
```

#### Study Drills

1. Modify one variable and re-run.
2. Break the code (missing brace, wrong type) and read the compiler error.
3. Add a feature of your own.
4. Comment every line in your copy.

---

## 🧠 Sample Complete Lesson

### **Exercise 1 – Hello, Go!**

**Goal:** Understand Go’s program structure and `fmt.Println`.

#### Code

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, Go!")
}
```

#### Run

```bash
go run ex01_hello.go
```

#### Output

```
Hello, Go!
```

#### Study Drills

1. Change the string to your own name.
2. Remove a brace and watch Go’s error message.
3. Build a binary:

   ```bash
   go build ex01_hello.go
   ./ex01_hello
   ```
4. Copy this file to `~/bin/` and run it from anywhere.

---

## 🧩 Study Drill Pattern

Every exercise ends with:

* **Type** the entire program manually.
* **Break** it intentionally to understand compiler feedback.
* **Run** it multiple times with changes.
* **Document** what you learned in comments.

---

## ☁️ Final Project

In Part 4 you’ll combine everything into a **DevOps Toolkit** binary that can:

* Parse CLI flags (`cobra`)
* Read configs (JSON/YAML)
* Manage AWS S3 or EC2 via SDK
* Interact with Docker/Kubernetes
* Expose `/metrics` for Prometheus
* Run concurrently with goroutines
* Handle graceful shutdown with contexts
* Log everything to file

Build once, run anywhere — even in a minimal container.

---

## 📄 License

MIT License — free for learning and teaching.

---

## 💬 Acknowledgment

Inspired by Zed A. Shaw’s *Learn Python the Hard Way*
and rewritten for the Go community by Ashraf Minhaj 💻

```
