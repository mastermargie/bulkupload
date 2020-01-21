# bulkupload
	Needs a valid API user account within the organization in which the API calls will be made.
	
	API Credentials must be generated and added as a profile to ./credentials (same directory where the container is run from), in the form of:
	[profile_name]
	VERACODE_API_KEY_ID=key_goes_here
	VERACODE_API_KEY_SECRET=secret_goes_here
	
	There can be multiple profiles in one file!
	
	Takes in a CSV file, wherein each row is a  call to be made and each column is a parameter to be passed to the call
	There must be a column called 'apiaction', where the cell is the API call to be made without the '.do' at the end
	See the sample.csv for more details
