# asciidoctor-ruby-portable

# How I created a portable basic ruby with Asciidoctor installed for Windows


## Steps

### 1. Download RubyInstaller for Windows WITHOUT DEVKIT

* https://rubyinstaller.org/downloads/
* Without Devkit to keep the size smaller ... ex. I didn't need the MSYS2 stuff.
* At the time of this writing the latest version: 3.1.2-1
* [Link to specific version](https://github.com/oneclick/rubyinstaller2/releases/download/RubyInstaller-3.1.2-1/rubyinstaller-3.1.2-1-x64.exe)

### 2. Run installer.

* Pointed installer to a folder on my desktop.

### 3. Install asciidocotor via gem 

* Navigate to the \Ruby31-x64\bin folder in a command prompt window and run the following to install Asciidoctor:

TIP: typing "cmd" in the address bar of Windows File Explorer will open cmd to the current folder.

```
C:\Users\<username>\Documents\Ruby31-x64\bin>gem install asciidoctor
```

Once finished query asciidoctor for the current version.

```
C:\Users\<username>\Documents\Ruby31-x64\bin>asciidoctor --version
```

### 4. Now we can run asciidoctor and convert .adoc files into html files.  I did not try to convert to anything else, such as pdf.

```
C:\Users\<username>\Documents\Ruby31-x64\bin>asciidoctor path/name/to_your_adoc_file.adoc
```
