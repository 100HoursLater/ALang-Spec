# REGEXP 
regexp in alang can be accessed with `std` 

`std.regexp().text()` this requires a string to be inserted in it => {
 - `/text/` is the text to be regular expression'd 
 - `/g` means global, it doesn't matter where or what case it is that is found, it is replaced by the following `.replace()` if it's present
 - `/ci` means case insensitive, when declared inside of the text portion it tells the following `.replace` to ignore case
 - `/edc` means exclude diacritics (this not excluded by defualt)
 - `.*` (this goes inside of the main `.text()` body where text normally should, this is wildcard.
}
 `std.regexp.text().replace()` this requires a string to be inserted in it => {
 - you can put the flags either side in the text portion or the replace side, the outcome is the same both times
}
