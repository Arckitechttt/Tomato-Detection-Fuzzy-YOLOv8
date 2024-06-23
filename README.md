# TomaTect: A GUI for Fresh / Rotten Tomato Detection with Combined Fuzzy and YOLOv8 Algorithms

**Description:**

The model used in this GUI (TomaTect App) is a combined Fuzzy and YOLOv8 algorithms named `Fuzzy YOLOv8.pt` that could detect fresh / rotten tomato from a picture of tomato.

**Steps to use the GUI:**
1. Your Python's version must be **3.10 <= Version < 3.12**
2. Open Windows Terminal / Powershell
3. `pip install ultralytics==8.0.48`
4. `pip install pyside6==6.4.2`
5. Go to your preferred directory path to clone this Repository using `cd [directory path]`
6. `git clone [repository URL]`
7. `cd Tomato-Detection-Fuzzy-YOLOv8`
8. `python main.py`

**Notes:**
1. If you want to use your own trained YOLOv8 model, you should put your `.pt` file (which you usually know as `best.pt` file) into the `models` folder.
2. If you checked the Save settings, the detection results will be saved in the `run` folder.
3. The UI design file is `home.ui` file, structured in PySide6. If you modify this file, you should run `pyside6-uic -o ui/home.py home.ui` in your Windows Terminal / Powershell, then change `import resources_rc` into `import ui.resources_rc` in line 23 of the `home.py` file, then run `python main.py` again to see the result.
4. The resource file is `resources.qrc` file. If you modify, delete, or add new images files path in this file, you should run `pyside6-rcc -o ui/resources_rc.py resources.qrc` in your Windows Terminal / Powershell, then run `python main.py` to see the result.
5. The version of your Python, Ultralytics, and PySide6 must be the same as mentioned in "Steps to use the GUI".
6. The `ultralytics` library follows the GPL-3.0 License (GNU General Public License Version 3), so if you need commercial use, you need to obtain its license first.

**References:**
1. https://ieeexplore.ieee.org/document/7103952
2. https://github.com/ultralytics/ultralytics
3. https://docs.ultralytics.com/
4. https://github.com/Jai-wei/YOLOv8-PySide6-GUI/