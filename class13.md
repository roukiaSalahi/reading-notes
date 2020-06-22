# HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

- the DHTML Behaviors include a userData behavior which allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.
- In 2002, Adobe introduced a feature in Flash which allows Flash objects to store up to 100 KB of data per domain.
- In 2007, Google launched Gears which can store unlimited amounts of data per domain in SQL database tables.

# HTML5 STORAGE

it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

HTML5 Storage supports the latest version of pretty much every browser 

## check for HTML5 Storage

```javascript

function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}

```
## USING HTML5 STORAGE

```javascript

var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;

```

***NOTE : the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.***

### to delete all the keys and values 

```javascript

interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};

```
### to get the name of each key

```javascript

interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};

```
## TRACKING CHANGES TO THE HTML5 STORAGE AREA

```javascript

if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};

```

PROPERTY  |	TYPE	 | DESCRIPTION
----------|----------|-------------------------------------------------------------------------
key	      | string   | the named key that was added, removed, or modified
oldValue  |	any	     | the previous value (now overwritten), or null if a new item was added
newValue  |	any      | the new value, or null if an item was removed
url       |	string   | the page which called a method that triggered this change

## HTML5 STORAGE IN ACTION

```javascript

function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}

```