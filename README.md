



</details>
<details>
<summary><b>Install OpenCV</b></summary>

**Any installation method is fine.**

Recommended:

```bash
python3 -m pip install --user --upgrade pip
python3 -m pip install --user opencv-python
python3 -m pip install --user opencv-contrib-python
```

More details on pip install openCV [here](https://www.pyimagesearch.com/2018/09/19/pip-install-opencv/).

</details>

<details>

<summary><b>Extra steps(for Linux users only)</b></summary>

<b>Installing missing libraries(if any):</b>

On a fresh computer, some of the libraries may get missing in event after a successful pip install. Install them using following commands[(ref)](https://www.pyimagesearch.com/2018/05/28/ubuntu-18-04-how-to-install-opencv/):

```bash
sudo apt-get install -y build-essential cmake unzip pkg-config
sudo apt-get install -y libjpeg-dev libpng-dev libtiff-dev
sudo apt-get install -y libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
sudo apt-get install -y libatlas-base-dev gfortran
```

</details>

### 2. Install project dependencies

Clone the repo

```bash
git clone https://github.com/Udayraj123/OMRChecker
cd OMRChecker/
```

Install pip requirements

```bash
python3 -m pip install --user -r requirements.txt
```

_**Note:** If you face a distutils error in pip, use `--ignore-installed` flag in above command._

<!-- Wiki should not get cloned -->

### 3. Run the code

1. First copy and examine the sample data to know how to structure your inputs:
   ```bash
   cp -r ./samples/sample1 inputs/
   # Note: you may remove previous inputs (if any) with `mv inputs/* ~/.trash`
   # Change the number N in sampleN to see more examples
   ```
2. Run OMRChecker:
   ```bash
   python3 main.py
   ```

Alternatively you can also use `python3 main.py -i ./samples/sample1`.

Each example in the samples folder demonstrates different ways in which OMRChecker can be used.

### Common Issues

<details>
<summary>
	1. [Windows] ERROR: Could not open requirements file<br>
	</summary>
Command: <code>python3 -m pip install --user -r requirements.txt</code>
<br>
	Link to Solution:  <a href="https://github.com/Udayraj123/OMRChecker/issues/54#issuecomment-1264569006">#54</a>
</details>
<details>
<summary>
2. [Linux] ERROR: No module named pip<br>
</summary>
Command: <code>python3 -m pip install --user --upgrade pip</code>
<br>
	Link to Solution: <a href="https://github.com/Udayraj123/OMRChecker/issues/70#issuecomment-1268094136">#70</a>
</details>

## OMRChecker for custom OMR Sheets

1. First, [create your own template.json](https://github.com/Udayraj123/OMRChecker/wiki/User-Guide).
2. Configure the tuning parameters.
3. Run OMRChecker with appropriate arguments .
<!-- 4. Add answer key( TODO: add answer key/marking scheme guide)  -->





