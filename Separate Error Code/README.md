# Separate Error Codes

## 📌 Description
This project Separate error codes stored in an array of strings based on their type ("Ax", "Bx", or "Cx") and store them in three different arrays.

## Activities Used
- Assign
- For each 
- Switch


## Explanation
- Created an Array of Strings variable ErrorCodes and the default value of: {"Ax001","Ax002","Ax003","Ax004","Ax005","Bx001","Bx002","Bx003","Cx001","Cx002","Cx003","Cx004"}.
- Created three Array of Strings variables, called AxArray, BxArray, and CxArray, and instantiated them with the default value: new string(){}.
- Added a for each loop to iterate through the ErrorCodes: ForEach currentText In ErrorCodes.
- Added a Switch inside the loop. Set the Expression to extract the first 2 letters using the 'Substring' method: currentText.Substring(0,2).ToLower. 
- For the Default case, added a Warn level Log Message with the Message: "No corresponding error code was found for: " + currentText.
- For each of the three cases ("ax", "bx", "cx"), used the 'Concat' method to add the item to the corresponding Array: e.g., AxArray.Concat({currentText}).ToArray.
- After the For Each activity, added three Log Message activities to print the content of each of the three Arrays, by using the 'String.Join' method: e.g., string.Join(" ",BxArray). 

