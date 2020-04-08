# Clean Code Javascript

## Index

- 1. Introduction
- 2. Variables
- 3. Fucntions
- 4. Objects and Data Structures
- 5. Classes
- 6. SOLID
- 7. Testing
- 8. Concurrency
- 9. Error Handling
- 10. Formatting
- 11. Comments

## 01. Introduction

This version is the Eddie's version of clean-code-javascript.
This is **not mendatory** to follow. There always be better way.

## 02. Variables

Naming Variables should be simple, easy and meaningful.

### 02-01 Use meaningful and easy to speak word to make variable's name

Bad Example:

```javascript
const yyyymmdstr = moment().format("YYYY/MM/DD");
```

Good Example:

```javascript
const currentDate = moment.format("YYYY/MM/DD");
```

### 02-02 Stay with same naming variables

Bad Examples:

```javascript
getUserInfo();
getClientData();
getCustomerRecord();
```

Good Example:

```javascript
getUser();
```

### 02-03 Use searchable name

Bad Example:

```javascript
// What the hell is 86400000?????
setTiemout(blastOff, 86400000);
```

Good Example:

```javascript
const MILLISECONDS_IN_A_DAY = 86400000;
setTimeout(blastOff, MILLISECONDS_IN_A_DAY);
```

### 02-04 Use recognizable variable name

Bad Example:

```javascript
const locations = ["Seoul", "Busan", "Suwon"];
locations.forEach((l) => {
  // ...
  // ...
  // what is l..?
  dispatch(l);
});
```

Good Example:

```javascript
const locations = ["Seoul", "Busan", "Suwon"];
locations.forEach((location) => {
  // ...
  // ...
  // better
  dispatch(location);
});
```

### 02-05 Stay simple

Bad Example:

```javascript
const Car = {
  carMake: "BMW",
  carModel: "M3",
  carColor: "blue",
};
```

Good Example:

```javascript
const Car = {
  make: "BMW",
  model: "M3",
  color: "blue",
};
```

### 02-06 Don't use es5 version of default parameter

Bad Example:

```javascript
function createMicro(name) {
  const breweryName = name || "Hipster";
}
```

Good Example:

```javascript
function createMicro(name = "Hipster") {}
```

## 03. Functions

## 04. Objects and Data Structures

## 05. Classes

## 06. SOLID

## 07. Testing

## 08. Concurrency

## 09. Error Handling

## 10. Formatting

## 11. Comments
