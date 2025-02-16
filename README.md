We firstly used ngrok to create link available for each other but to continue the work in our side we use local links

In order to launch all APIs, open the project and write the following on a terminal:

Start-Process python -ArgumentList "api_cnn.py"
Start-Process python -ArgumentList "api_lstm.py"
Start-Process python -ArgumentList "api_dnn.py"
Start-Process python -ArgumentList "api_rf.py"
Start-Process python -ArgumentList "api_svm.py"

If it doesn't works, simply run the files in differents terminals.

Then in another terminal, run the aggregate_model.py to do the concensus prediction :

python aggregate_model.py
