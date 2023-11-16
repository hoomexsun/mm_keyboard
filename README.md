# kybd-mm

Meetei/Meitei Mayek Character Keyboard.

This repository contains resources from which you can extract and install Meetei Mayek keyboard in Windows/Ubuntu.

- Download and install `khut_e.zip` for windows
- Download and install `Eeyek-2.0.zip` for ubuntu (Built by [Tabish](http://tabish.freeshell.org/eeyek/download.html))

## 1. Keyboard Layout (khut_e)

### 1.1. Normal Mode

![khut_e keys SHIFT Mode](./images/khut_e_keys.png)

### 1.2. Shift Mode

Hold `Shift` and Type.

![khut_e keys ShiftMode](./images/khut_e_keys_shift.png)

### 1.3. Ctrl Mode

Hold `Ctrl` and Type. (Might not probably work if `Ctrl` is bound as part of shortcuts, eg., `Ctrl`+`Z` is undo so typing `Z` might not work.)

![khut_e keys Ctrl Mode](./images/khut_e_keys_ctrl.png)

## 2. Instructions

1. Download and extract **khut_e.zip**
2. Run `setup.exe` and install the khut_e font.
3. Press `Windows` + `Space` to change Language
   ![Choosing Language](./images/choosing_lang.png)
4. You can type in **MS Office** apps by default (MS Word, MS Powerpoint, MS Excel) but if the glyphs are not visible in **notepad** (if it shows boxes instead of the correct characters), you can fix it by typing using the font in any other app which can display Meitei Mayek by default. (Eg., MS Word)

## 3. Fonts

Nirmala UI supports Meetei/Meitei Mayek by default in windows. But it is preferred to download and install [Noto Sans Meetei Mayek](https://fonts.google.com/noto/specimen/Noto+Sans+Meetei+Mayek) from Google Fonts.

This repository also contain a copy of [Eeyek font](http://tabish.freeshell.org/eeyek/download.html) which can be used to type Meetei/Meitei Mayek in Ubuntu OS.

![Eeyek Layout](./images/eeyek_layout.png)

## 4 Typing in LaTeX

1. Install [MikTeX](https://miktex.org/download) and [TexMaker](https://www.xm1math.net/texmaker/download.html) to edit LaTeX files.
2. Install Meetei Mayek Unicode fonts ([Noto Sans Meetei Mayek](https://fonts.google.com/noto/specimen/Noto+Sans+Meetei+Mayek)).
3. Install `khut_e` to type Meetei Mayek Unicode in Windows.
4. Make the following changes (highlighted)
   a. Create a new LaTeX file and add fontspec package.
   b. Create a new font family, add a preferred name (eg., \MM) and use Noto Sans Meetei Mayek (check spelling and cases).
   c. Use {\MM type the chracters here}
   d. You can type the characters using Khutyee in windows or using Eeyek in Ubuntu
   e. You can also use LaTeX \char to type the characters using the actual Unicode values.

   ```latex
   \documentclass[12pt,a4paper]{article}
   \usepackage{fontspec}
   \newfontfamily\MM{Noto Sans Meetei Mayek}

   \begin{document}

   {\MM
   ꯀ ꯁ ꯂ ꯃ ꯄ ꯅ
   \char"ABC0
   }

   \end{document}
   ```

5. Change Compiler of Tex file in TexMaker to XeTeX or LuaTeX to use fontspec.
6. In Word Processor like MS Word, WordPad etc. Nirmala UI, Eeyek or Noto Sans Meetei Mayek is required to show the proper glyphs (else Unicode empty blocks will show up).
7. Same steps for **TexMaker** and **Overleaf** (Don’t forget to change compiler to **LuaLaTeX**).

_Example_
![texmaker](./images/texmaker_ss_1.png)

### 4.1. Overleaf

_1. Setting Compiler to LuaLaTeX in Overleaf_
![overleaf](./images/overleaf_ss_1.png)

_2. Output pdf_
![overleaf](./images/overleaf_ss_2.png)

### 4.2. TexMaker

_1. Setting Compiler to LuaLaTeX in TexMaker_
![texmaker](./images/texmaker_ss_2.png)

_2. Output pdf_
![texmaker](./images/texmaker_ss_3.png)

## 5. FAQs

### 5.1. Typing in Google Chrome

1. **Settings** > **Appearance** > **Customize fonts** or type **chrome://settings/fonts** in search bar and press `Enter`
2. **Customize fonts** > **Standard font** > pick **Noto Sans Meetei Mayek**

![Chrome 1](./images/chrome_1.png)

3. Screenshot of Typing

![Chrome 1](./images/chrome_2.png)

### 5.2. Typing in VS Code

1. Click on **File**

![VSCode 1](./images/vscode_1.png)

2. Go to **Preferences**

![VSCode 1](./images/vscode_2.png)

3. Go to **Settings**

![VSCode 1](./images/vscode_3.png)

4. Add **Noto Sans Meetei Mayek** in **Font** of **User** Settings

![VSCode 1](./images/vscode_4.png)

5. Screenshot of Typing

![VSCode 1](./images/vscode_5.png)

### 5.3. Typing in Google Collab/Jupyter Notebook

Similar to **Section 4.1.**

### 5.4 How do i go back to my usual keyboard?

Press `Windows` + `Space` again till you change it back.

## Warning

- The character in the keyboard is not in the default system code page (1252) of the English (India) language you specified. This may cause compatibility problems in non-Unicode applications.

## See also

- [Speech Dataset](https://github.com/hoomexsun/speech_dataset).
- [Meetei/Meitei Mayek Transliteration](https://github.com/hoomexsun/mm_transliteration).
- [Meetei/Meitei Mayek Keyboard for Windows](https://github.com/hoomexsun/mm_keyboard).
- [IPA Keyboard for Windows](https://github.com/hoomexsun/ipa_keyboard).
- [S-550 Glyph Correction](https://github.com/hoomexsun/s550_glyph_correction).
- [Epaomayek Glyph Correction](https://github.com/hoomexsun/epaomayek_glyph_correction).
- [Microsoft Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134)

```

```
