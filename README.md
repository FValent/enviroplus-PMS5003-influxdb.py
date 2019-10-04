# enviroplus-PMS5003-influxdb.py
Get data from EnviroPlus sensor board with PMS5003 particulate sensor and put them on influxdb.
Need a Raspberry Pi (Zero with Wireless, It's enough).

Prerequisite clone and install everything need from pimoroni/enviroplus-python, then add influxdb and pip install influxdb.
Be sure influxdb is running.
You can create an influxdb database using cli and add a user with password and put this on run.py.

On Raspberry Pi console, after running the run.py you should see something like this:
Write points: [{'fields': {'bme280.temperature.compensated': 1.2989094609770326, 'bme280.pressure': 923.8708401231879, 'pms5003.pm010': 3, 'pms5003.pm100': 4, 'mics6814.nh3': 3793999.9999999967, 'ltr559.proximity': 60, 'pms5003.pm025': 4, 'ltr559.lux': 1.0, 'mics6814.oxidising': 99555.55555555558, 'bme280.temperature.raw': 14.17729309376757, 'bme280.humidity': 43.981306005167795, 'cpu.temperature': 23.9, 'mics6814.reducing': 514370.3703703706}, 'tags': {'host': 'enviroplus'}, 'measurement': 'enviroplus'}]



