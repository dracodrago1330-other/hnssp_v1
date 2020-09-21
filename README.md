# Hungarian Notation / Sigil / Suffix Based Language (mega-alpha _v_.1)



## Sigils for types



#### numeric types

`#Int` = `int Int;`

`##Long` = `long int Long;`

`###LongLong` = `long long LongLong;`

`#.Float` = `float Float;`

`#..Double` = `double Double;`

`##..LongDouble` = `long double LongDouble;`



#### character-like types

`'Char` = `char Char;`

`"String` | `"(String With Spaces)` = `const char* String;`





```
->"SuccessorOfString( @"Str ) {
	[ MappingArray ] @Str.split "();;

	map_over MappingArr with 'CurrentChar {
		'(CurrentChar.ord + 1);
	}

	MappingArr.join "();;
}
```

```
::Error() {
	raise _Error.init "Error";;
	_Program.quit;;
}

&::ErrorOnFloat(uniTest{ T }) {
	if Test.type is #.T {
		Error;;
	}
}

->Main() {
	for uniCurrentElement{ #T, #.T } of ([ #1, #2, #3, #4, #5, #6, #7, #.8 ]) {
		ErrorOnFloat CurrentElement;;
	}
}
```

