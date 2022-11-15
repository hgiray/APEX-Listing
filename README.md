# APEX-Listing
How to write list code in APEX
//List class
List<string> Cars = new List<string>();
Cars.add('Tesla');
Cars.add('Toyota');
Cars.add('Cadillac');
Cars.add('Ferrari');
system.debug('Model ' +Cars);
system.debug('size of the list ' +Cars.size());
system.debug('secondCall '+Cars.get(1));
Integer Result = Cars.indexof('Cadillac');
system.debug('Favorite Car ' +Result);
Cars.set(1, 'Mercedes');
System.debug('Replace toyota to mercedes ' +Cars);
Cars.remove(1);
system.debug('Delete the mercedes ' +Cars);
Cars.clear();
system.debug('Delete the whole list '+ Cars);
//Set class
Set<string> Colors = new Set<string>();
Colors.add('Green');
Colors.add('Blue');
Colors.add('Orange');
Colors.add('Red');
system.debug('Colors ' +Colors);
system.debug('The size of set '+Colors.size());
Colors.remove('Green');
system.debug('Delete my favorite color ' +Colors);
Colors.clear();
System.debug('Delete my favorite color '+Colors);
//Map class
Map<String,string> capitalCountry = new Map<string,string>();
capitalCountry.put('Turkey','Ankara');
capitalCountry.put('USA','Washington');
capitalCountry.put('Germany','Berlin');
capitalCountry.put('Canada','Ottawa');
system.debug('Countries and capitols '+capitalCountry);
Set<string>Countries = new Set<string>();
Countries=capitalCountry.keyset();
system.debug('Keys of set '+Countries);
List<string>Capitals = new List<string>();
Capitals=capitalCountry.values();
system.debug('Values of list '+Capitals);
system.debug('The size of new list '+capitalCountry.size());
capitalCountry.remove('Turkey');
system.debug('Delete turkey '+capitalCountry);
Map<string,string>centralCountry=capitalCountry.clone();
system.debug('Clone the map '+centralCountry);
system.debug('Get the capital of germany '+capitalCountry.get('Germany'));
capitalCountry.clear();
system.debug('Delete the whole list '+capitalCountry);
