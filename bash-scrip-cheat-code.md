Here’s your **Day 4 — Bash Scripting Basics Cheat Sheet** that you can add to your GitHub repo just like we did for Day 3.

---

## **`day4-bash-scripting-cheatsheet.md`**

````markdown
# Day 4 — Bash Scripting Basics Cheat Sheet

## 1. Script Structure
```bash
#!/bin/bash    # Shebang - tells the system to use Bash
# This is a comment

echo "Hello World"   # Print text to screen
````

## 2. Running Scripts

```bash
chmod +x script.sh   # Make executable
./script.sh          # Run script in current directory
bash script.sh       # Run script with bash
```

## 3. Variables

```bash
name="Phillip"
echo "Hello $name"
```

## 4. Command Substitution

```bash
today=$(date)
echo "Today is $today"
```

## 5. Positional Parameters

```bash
#!/bin/bash
echo "First argument: $1"
echo "Second argument: $2"
```

Run:

```bash
./script.sh arg1 arg2
```

## 6. Conditionals

```bash
if [ $1 -gt 10 ]; then
    echo "$1 is greater than 10"
else
    echo "$1 is 10 or less"
fi
```

## 7. Loops

```bash
for i in {1..5}; do
    echo "Number $i"
done
```

## 8. Functions

```bash
greet() {
    echo "Hello $1"
}
greet Phillip
```

## 9. Reading User Input

```bash
read -p "Enter your name: " name
echo "Hello $name"
```

## 10. Useful Commands in Scripts

```bash
pwd      # Current directory
ls       # List files
whoami   # Current user
uptime   # System uptime
```

---

**Pro Tips:**

* Always start with `#!/bin/bash`
* Use `chmod +x` before running
* Test scripts in a safe environment before production

```

