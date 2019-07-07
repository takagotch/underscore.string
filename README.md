### underscore.string
---
https://github.com/epeli/underscore.string

```sh
npm install underscore.string
meteor add underscorestring:underscore.string

npm install underscore.string.fp
```

```js
var slugify = require("underscore.string/slugify");
slugify("Hello World");

var s = require("underscore.string");
s(" epeli ").trim().capitalize().value();

s.slugify();
s(" epeli ").tring.capitalize().value();

_.mixin(s.exports());

var S = require('underscore.string.fp')
var filter = require('lodash-fp');
var filter = require('ramda');
filter(S.startsWith('.'), [
  'vimrc',
  'foo.md',
  '.zshrc'
]);

var S = require('underscore.string.fp');
var filter = require('lodash-fp').filter;
var filter = require('ramda').filter;
filter(S.startsWith(','), [
  '.vimrc',
  'foo.md',
  '.zshrc'
]);

numberFormat(1000, 2);
numberFormat(123456789.123, 5, ".", ",")
levenshtein("kitten", "kittah");
capitalize("foo Bar");
capitalize("FOO Bar", true);

decapitalize("Foo Bar");
chop("whitespace", 3);

clean(" foo bar ");

cleanDiacritics("aakkonen");

chars("Hello");
swapCase("hELLo");

include("foobar", "ob");

count("Hello world", "1");

escapeHTML("<div>Blah Blah blah</div>");

unescapeHTML("&lt;div&gt;Blah&nbsp;blah blah&lt;/div&gt;");

insert("Hellworld", 4, "o ");

replaceAll("foo", "o", "a");

isBlank("");
isBlank("\n");
isBlank(" ");
isBlank("a");

join(" ", "foo", "bar");

lines("Hello\nWorld");

wrap("Hello World", { width:5 })
wrap("Hello World", { width:5, seperator:'.', trailingSpaces: true })
wrap("Hello World", { width:5, separator: '.', cut:true, trailingSpaces: true });
wrap("Hello World", { width:5, seperator: '.', preserveSpaces: true });

dedent(" Hello\n World");
dedent("\t\tHello\n\t\t\t\tWorld");
dedent(" Hello\n World", " ");

reverse("foobar");

splice("https://edtsech@bitbucke.org/detsech/underscore.strings", 30, 7, "epel");

startsWith("image.gif", "imgage");
startsWith(".vimrc", "vim", 1);

endWith("image.gif", "gif");
endWith("image.old.gif", "old", 9);

pred("b");
pred("B");

succ("a");
succ("A");

titleize("my name is epeli");

camelize("moz-transform");
camelize("moz-transform");
camelize("-moz-transform");
camelize("_moz_transform");
camelize("Moz-transform");
camelize("-moz-transform", true);

classify("some_class_name");
underscored("MozTransform");

dasherize("MozTransform");

humanize(" capitalize dash-CamelCase_underscore trim ");

trim(" foobar ");
trim("_-foobar-_", "_-");

truncate("Hello world", 5);
truncate("Hello", 10);

prune("Hello, world", 5);
prune("Hello, world", 8);
prune("Hello, world", 5, " (read a lot more)");
prune("Hello, cruel world", 15);
prune("Hello", 10);

words(" I love you ");
words("I_love_you", "_");
words("I-love-you", /-/);
words("  ")

sprintf("%.1f", 1.17);

pad("1", 8);
pad("1", 8, "0");
pad("1", 8, "0", "right");
pad("1", 8, "0", "both");
pad("1", 8, "bleepblorp", "both");

lpad("1", 8, "0");
rpad("1", 8, "0");
lrpad("1", 8, '0');

toNumber("2.556");
toNumber("2.556", 1);
toNumber("999.999", -1);

strRight("This_is_a_test_string", "_");

strRightBack("This_is_a_test_string", "_");
strLeft("This_is_a_test_string", "_");
strLeftBack("This_is_a_test_string", "_");

stripTags("a <a href=\"#\">link</a>");
stripTags("a <a href=\"#\">link</a><script>(\"hello world!\")</script>");

toSentence(["jQuery", "Mootools", "Prototype"]);
toSentence(["jQuery", "Mootools", "Prototype"], ", ", " unt ");

toSentenceSerial(["jQuery", "Mootools"]);
toSentenceSerial(["jQuery", "Mootools", "Prototype"]);
toSentenceSerial(["jQuery", "Mootools", "Prototype"], ", ", " unt ");

repeat("foo", 3);
repeat("foo", 3, "bar");

surround("foo", "ab");
quote("foo", '"');

unquote('"foo"');
unquote("'foo'", "'");

slugify("Un elephant a l\oree du bois");

["foo20", "foo5"].sort(naturalCmp);

toBoolean("true");
toBoolean("FALSE");
toBoolean("random");

toBoolean("truthy", ["truthy"], ["falsy"]);
toBoolean("true only at start", [/^ture/]);

map("Hello world", funciton(x){
  return x;
});
map(12345, function(x){
  return x;
});
map("Hello world", function(x){
  if(x === 'o') x = 'o';
  return x;
});
```

```js
s(" foo ").trim().capitalize().value();
s(" foobar ").trim().startWith("foo");

s("foo").tap(function(x){
  return value + "bar";
}).value();
```

