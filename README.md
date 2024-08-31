<p align="center">🛡️ Nuitka & Protection Guide 🛡️</p>
<br><br>

<p align="center"><strong>This repository explains how to use Nuitka to compile your Python scripts into standalone executables and apply advanced protection with VMProtect, Themida, or similar tools.<br><br>By following this guide, you can distribute your Python programs while protecting them from reverse engineering.<br><br></strong></p>
<br>

<p align="center">📀 Example Scripts 📀</p>
<p align="center"><strong><i>Here are some example scripts to demonstrate the compilation and protection process.</i></strong></p>
<br><br>

<p align="center">simple_script.py</p>
<p align="center"><strong><i>This is a simple Python script that prints "Hello, World!" to the console.</i></strong></p>

<pre>
<code>
print("Hello, World!")
</code>
</pre>
<br><br>

<p align="center">advanced_script.py</p>
<p align="center"><strong><i>This is a more complex script that might include external dependencies and requires additional considerations when converting to an executable.</i></strong></p>

<pre>
<code>
import os

def main():
    print(f"Current working directory: {os.getcwd()}")

if __name__ == "__main__":
    main()
</code>
</pre>
<br><br>

<p align="center">🛠️ How to Compile and Protect a Python Script 🛠️</p>
<br><br>

<p align="center"><strong><i>Follow these steps to compile your Python script into an executable and protect it from reverse engineering:</i></strong></p>
<br><br>

<h3>Step 1: Compile with Nuitka</h3>

<ol>
  <li>Install Nuitka via pip:
    <pre><code>pip install nuitka</code></pre>
  </li>

  <li>Navigate to the directory containing your script:
    <pre><code>cd path/to/your/script</code></pre>
  </li>

  <li>Compile the script using Nuitka:
    <pre><code>nuitka --standalone --onefile --output-dir=output_dir your_script.py</code></pre>
    This will create a standalone executable in the <code>output_dir</code>.
  </li>
</ol>

<h3>Step 2: Protect with VMProtect or Themida or other protector</h3>

<p>Once you have generated the executable with Nuitka, you can use VMProtect or Themida to protect it:</p>

<h4>VMProtect:</h4>
<ol>
  <li>Open VMProtect and select the compiled executable.</li>
  <li>Configure the protection settings according to your needs.</li>
  <li>Generate the protected executable.</li>
</ol>

<h4>Themida:</h4>
<ol>
  <li>Open Themida and import the executable.</li>
  <li>Configure the desired protection options.</li>
  <li>Apply the protection and save the output.</li>
</ol>
<br><br>

<p align="center">🔒 Why Use VMProtect or Themida? 🔒</p>
<br><br>

<p>These tools add layers of protection to your executables, making it much harder for attackers to reverse engineer your code. They offer various features such as code obfuscation, anti-debugging mechanisms, and virtualization.</p>

<br><br>

<p align="center">🗂️ Additional Resources 🗂️</p>
<br><br>

<p>For more details on how to bundle your Python application with Nuitka, refer to the official documentation:</p>

<p align="center"><a href="https://nuitka.net/doc/bundles.html">Nuitka Bundles Documentation</a></p>

<br><br>

<p align="center">README.md inspired by <a href="https://github.com/billythegoat356/">this repo</a></p>
