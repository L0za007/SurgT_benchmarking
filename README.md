# SurgT_benchmarking

A tool to benchmark tissue trackers in surgery.

# How to run the code

Here, I will assume that you are using python 3.9.
If you are using other versions you may need to adapt the library versions on the `requirements.txt`.

Create a Python virtual environment:
```
python3.9 -m pip install --user virtualenv
python3.9 -m virtualenv venv
```

Then you can activate that environment and install the requirements using:
```
source venv/bin/activate
pip install -r requirements.txt
```

Now, when the `venv` is activated you can run the code using:

```
python main.py
```

This by default will download the data for you.

# How to assess your own method?

As you can see from `main.py` this code will be calling the function `run_method()` from the file `code/method.py`.
There we show an example of an OpenCV 2D tracker that is benchmarked in our dataset. You can use the same functions to assess your own method.

# Submission instructions

At the end of the MICCAI SurgT challenge, we expect you to send us a docker image file containing this tool `SurgT_benchmarking` already set-up for your own method.
Then we will simply add the links to the test data and run the `main.py` to get the final results. You will only be ranked given your results on the test data.
The test data links will not be available to you until the end of the competition.
