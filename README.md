# Regex for IP addresses
This readme file explains how to use regular expressions to detect an IP address in a log file.

## Summary
The following regular expression is for detecting IP addresses in a text file (generally in router logs forwared to a syslog server).

```
/(?P<router_wan_ip>^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}$)/gm
```

a sample log -
```
2021-05-20 05:16:42 syslog-server ping alert normal core-net alex1 transit-net: [alex2] [intf-xe-5/1/0.0] cross-over LAN interface 192.56.208.2 down
```

Result -
![example](./assets/images/example.png)

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Generally regex is used to match a pattern. Anchors are different in the sense that they do not match any character, rather they match a position like before, after or between characters. Here are some of the commonly used anchors -

|Description | Symbol |
|-------------|--------|
|Start of string| ^|
|End of String| $ |
|Word Boundary| \b |


### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
