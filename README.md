# GPS Data Logger

This Python script reads GPS data from a serial port and extracts latitude and longitude information. It then converts this data into degrees and plots the location on Google Maps using a web browser.

## Requirements

- Python 3.x
- Serial library (should be installed by default)
- Webbrowser library (should be installed by default)

## Usage

1. Connect your GPS device to the appropriate serial port. Make sure to update the `ser = serial.Serial ("/dev/ttyS0")` line in the code with the correct serial port address.

2. Run the Python script.

3. The script will continuously read GPS data. When it receives valid GPS data, it will print the latitude and longitude in degrees and open a web browser to display the location on Google Maps.

4. Press `Ctrl+C` to stop the script and plot the last received location on Google Maps.

## Notes

- This script assumes that the GPS device outputs NMEA data in the GPGGA format. If your GPS device uses a different format, you may need to modify the code accordingly.
- Ensure that you have an active internet connection for the Google Maps plotting to work.

## References

- [Python Serial Library Documentation](https://pythonhosted.org/pyserial/)
- [Python Webbrowser Library Documentation](https://docs.python.org/3/library/webbrowser.html)
