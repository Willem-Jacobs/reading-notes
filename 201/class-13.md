# Class 13 Reading

[Return to 201 TOC](201TOC.md)

*Resource: <http://diveinto.html5doctor.com/storage.html>

## The Past, Present, and Future of Local Storage for Web APplications

- In the earlier days of web, browsers had minimal ability for some type of local storage. Mainly cookies were available but these had small amount of storage space and not secure. Developers created add-ons to use but these also had their set of issues.
- HTML5 added local storage and session storage.
- Local storage has more space, 5mb, available and uses a structure similar to an object of a key/value STRING record saved to the local storage of the browser. The value will always be a string when saved.
- The developer is to convert objects to strings using the JSON.stringify method and the JSON.parse method to convert the value back from a string to an object. Other values also need to be converted back from string to their required types.
- Local storage will presist after leaving a page and closing the browser but the drawback is anyonce can see this data in the inspector and can even change/delete the data. It is not secure.
- Local storage syntax is simple to use. To begin you call localStorage and then one of the 6 methods available. These are: `clear(), getItem(), key(), length(), removeItem(), setItem()`
- Clear is used to clear the entire local storage.
- getItem() is used to retrieve data from the local storage using the key assigned.
- key() is used to get the key value.
- length() is used to get the length of the local storage to see how many key/value entries. Similar to an array.
- removeItem() is used to remove the specified key item from the local storage.
- setItem() is used to set the item into the local storage by specifying a key value as a string and the data as the second parameter. Reminder that all values should be of string type. setItem() will try to convert to string as it automatically calls a .toString() methond but on objects, it can't convert so JSON has to be used. Booleans are also saved back as string.
- getItem() remember to convert the string values received back to the proper data type. JSON should be used for all retrival and parse it and convert other data types to int, boolean, etc.
- Local storage is array type so the [] can be used example: l`ocalStorage.setItem['key'] = 'the value to set';` or `let value = localStorage.getItem['key'];`.
- Event listener can be set on the local storage with the event type of 'storage'. Event object will be returned with properties of key, oldValue, newValue, url.
- A lite version of a SQL style storage was added to browsers but this is being removed in future.
- indexDB is a new method that browers now support. This works more like a database using a database name, table and key/value entries. The docs did not discuss much on this.

[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
