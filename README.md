Weather is a simple script that curls from wttr.in
in an attempt to pull your requested city's weather
forecast all from command line.  The script will
allow for a city and state, or a zip/postal code,
to be entered after the command [weather sacramento,
ca or weather 01902 will result in weather for each
respective area].  If no location information is
entered after the command, then it polls your public
IP address, performs a query of your IP address's
city, state, and zip code and uses that information
for its forecast query.

BUGS:
Currently, only US and Canada zip/postal codes are
accepted.  This is based on wttr.io capability of
searching based on postal code.  The result of
using a zip or postal code from other than US or
Canada is "ERROR" and exit.
There is also an issue performing this while using
a VPN connection or SSH Tunnels or Socks Proxy. The
public IP address of the VPN server will be used to
base location.
