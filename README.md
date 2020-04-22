# generate_vtf_fits_file

This code creates skeleton VTF FITS files with headers that are compliant with the YAML files in the DKIST fits-validator package. The files contain no image data.

Requirements:
* fits-validator
* pyyaml
* astropy

## Usage

Set up an environment with python (must be version >=3.7) and ensure the required libraries are installed:
```
pip install fits-validator pyyaml astropy
```

Then copy the `generate_vtf_fits_file.py` script to your machine and run it with
```
python generate_vtf_fits_file.py
```

## Changing the FITS keywords or values

You can modify the values or add new keywords by using the command
```
hdu.header['keyword_name'] = VALUE
```
in the section of the code where a number of examples have already been provided.

## Example
Running the script
```
>>> python generate_vtf_fits_file.py
File example_vtf_file.fits created.
```
Output FITS file headers
```
SIMPLE  =                    T / conforms to FITS standard                      
BITPIX  =                    8 / array data type                                
NAXIS   =                    0 / number of array dimensions                     
EXTEND  =                    T                                                  
AO___001=                 7.89                                                  
AO___002= 'default '                                                            
AO___003=                 7.89                                                  
AO___004=                 7.89                                                  
AO___005=                 7.89                                                  
AO___006=                 7.89                                                  
AO___007=                 7.89                                                  
AO___008=                 7.89                                                  
CAM__001= 'default '                                                            
CAM__002= 'default '                                                            
CAM__003=                    5                                                  
CAM__004=                 7.89                                                  
CAM__005=                 7.89                                                  
CAM__006=                 7.89                                                  
CAM__007=                    5                                                  
CAM__008=                    5                                                  
CAM__009=                    5                                                  
CAM__010=                    5                                                  
CAM__011=                    5                                                  
CAM__012=                    5                                                  
CAM__013=                    5                                                  
CAM__014=                    5                                                  
CAM__015=                    5                                                  
CAM__016=                    5                                                  
CAM__017=                    5                                                  
CAM__018=                    5                                                  
CAM__019=                    5                                                  
CAM__020=                    5                                                  
CAM__021=                    5                                                  
CAM__022=                    5                                                  
CAM__023=                    5                                                  
CAM__024=                    5                                                  
CAM__025=                    5                                                  
CAM__026=                    5                                                  
CAM__027=                    5                                                  
CAM__028=                    5                                                  
CAM__029=                    5                                                  
CAM__030=                    5                                                  
CAM__031=                    5                                                  
CAM__032=                    5                                                  
DKIST001= 'default '                                                            
DKIST002= 'default '                                                            
DKIST003= 'default '                                                            
DKIST004= 'default '                                                            
DKIST005= 'default '                                                            
DKIST006= 'default '                                                            
DKIST007=                    T                                                  
DKIST008=                    5                                                  
DKIST009=                    5                                                  
DKIST010=                    5                                                  
ID___001= 'default '                                                            
ID___002= 'default '                                                            
ID___003= 'default '                                                            
ID___004= 'default '                                                            
ID___005= 'default '                                                            
ID___006= 'default '                                                            
ID___007= 'default '                                                            
ID___008= 'default '                                                            
ID___009= 'default '                                                            
ID___010= 'default '                                                            
ID___011= 'default '                                                            
ID___012= 'default '                                                            
ID___013= 'default '                                                            
ID___014= 'default '                                                            
BUNIT   = 'default '                                                            
BZERO   =                    0                                                  
BSCALE  =                    1                                                  
BLANK   =                    0                                                  
DATE    = '2020-04-22T15:33:53'                                                 
DATE-OBS= '2020-04-22T15:33:53'                                                 
DATE-BGN= '2020-04-22T15:33:53'                                                 
DATE-END= '2020-04-22T15:33:53'                                                 
ORIGIN  = 'default '                                                            
TELESCOP= 'DKIST   '                                                            
OBSERVAT= 'National Solar Observatory'                                          
NETWORK = 'default '                                                            
INSTRUME= 'VTF     '                                                            
WAVELNTH=                 7.89                                                  
OBSERVER= 'default '                                                            
OBJECT  = 'default '                                                            
CHECKSUM= 'default '                                                            
DATASUM = 'default '                                                            
PAC__001= 'default '                                                            
PAC__002= 'default '                                                            
PAC__003= 'default '                                                            
PAC__004= 'default '                                                            
PAC__005= 'default '                                                            
PAC__006= 'default '                                                            
PAC__007= 'default '                                                            
PAC__008=                 7.89                                                  
PAC__009=                 7.89                                                  
PAC__010= 'default '                                                            
PAC__011=                 7.89                                                  
VTF__001= 'default '                                                            
VTF__002= 'default '                                                            
VTF__003=                    5                                                  
VTF__004=                    5                                                  
VTF__005=                 7.89                                                  
VTF__006=                 7.89                                                  
VTF__007=                    5                                                  
VTF__008= 'default '                                                            
VTF__009=                    5                                                  
VTF__010=                    5                                                  
VTF__011= 'default '                                                            
VTF__012= 'default '                                                            
VTF__013=                    5                                                  
VTF__014=                    5                                                  
VTF__015=                 7.89                                                  
VTF__016=                 7.89                                                  
VTF__017=                 7.89                                                  
VTF__018=                 7.89                                                  
VTF__019=                 7.89                                                  
VTF__020= 'default '                                                            
VTF__021=                    5                                                  
VTF__022=                    5                                                  
VTF__023=                 7.89                                                  
VTF__024=                 7.89                                                  
VTF__025=                 7.89                                                  
VTF__026=                    5                                                  
VTF__027=                    5                                                  
VTF__028=                    5                                                  
VTF__029=                    5                                                  
WCSAXESA=                    5                                                  
WCSAXESB=                    5                                                  
WCSNAMEA= 'default '                                                            
WCSNAMEB= 'default '                                                            
CRPIX1A =                 7.89                                                  
CRPIX2A =                 7.89                                                  
CRPIX3A =                 7.89                                                  
CRPIX1B =                 7.89                                                  
CRPIX2B =                 7.89                                                  
CRPIX3B =                 7.89                                                  
CRDATE1A= 'default '                                                            
CRDATE2A= 'default '                                                            
CRDATE3A= 'default '                                                            
CRDATE1B= 'default '                                                            
CRDATE2B= 'default '                                                            
CRDATE3B= 'default '                                                            
CRVAL1A =                 7.89                                                  
CRVAL2A =                 7.89                                                  
CRVAL3A =                 7.89                                                  
CRVAL1B =                 7.89                                                  
CRVAL2B =                 7.89                                                  
CRVAL3B =                 7.89                                                  
CDELT1A =                 7.89                                                  
CDELT2A =                 7.89                                                  
CDELT3A =                 7.89                                                  
CDELT1B =                 7.89                                                  
CDELT2B =                 7.89                                                  
CDELT3B =                 7.89                                                  
CUNIT1A = 'default '                                                            
CUNIT2A = 'default '                                                            
CUNIT3A = 'default '                                                            
CUNIT1B = 'default '                                                            
CUNIT2B = 'default '                                                            
CUNIT3B = 'default '                                                            
CTYPE1A = 'default '                                                            
CTYPE2A = 'default '                                                            
CTYPE3A = 'default '                                                            
CTYPE1B = 'default '                                                            
CTYPE2B = 'default '                                                            
CTYPE3B = 'default '                                                            
PCI_JA  =                 7.89                                                  
LONPOLEA=                 7.89                                                  
LONPOLEB=                 7.89                                                  
LATPOLEA=                 7.89                                                  
LATPOLEB=                 7.89                                                  
TAZIMUTH=                 7.89                                                  
TELEVATN=                 7.89                                                  
TELTRACK= 'default '                                                            
TELSCAN = 'default '                                                            
TTBLANGL=                 7.89                                                  
TTBLTRCK= 'default '                                                            
WFC__001=                 7.89                                                  
WFC__002=                    T                                                  
WFC__003= 'default '                                                            
WFC__004=                 7.89                                                  
WFC__005=                 7.89                                                  
WFC__006=                    5                                                  
WFC__007=                    T                                                  
WFC__008=                 7.89                                                  
WFC__009=                 7.89                                                  
WS___001= 'default '                                                            
WS___002=                 7.89                                                  
WS___003=                    5                                                  
WS___004=                 7.89                                                  
WS___005=                 7.89                                                  
WS___006=                 7.89                                                  
WS___007=                 7.89                                                  
COMMENT default
```
