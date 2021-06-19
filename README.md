# iOS Icon Generator
Bash Script to Generate iOS Scaled Icons (1x, @2x, @3x)

## How to use ## 

#### Setup ####

Makes the file executable and copies it to `/usr/local/bin` so it can be accessed from anywhere.

1. Clone this repo.
2. `cd ios-icon-generator`
3. `chmod +x igen`
4. `cp igen /usr/local/bin/igen`

#### Usage 1 ####

Use the default, `sunset.jpg` file in this repo.

__Command__
`igen sunset.jpg`

__Output__
```
Using 'sunset.jpg' to convert...
(3/3) Files Created Successfully!
1. sunset.jpg = 300 x 300
2. sunset@2x.jpg = 603.00 x 603.00
3. sunset@3x.jpg = 900 x 900
```

__Finder__
<img src="./example.png" width="400">

#### Usage 2 ####

__Command__
`igen sunset.jpg icon.jpg`

__Output__
```
Using 'sunset.jpg' to convert...
(3/3) Files Created Successfully!
1. icon.jpg = 300 x 300
2. icon@2x.jpg = 603.00 x 603.00
3. icon@3x.jpg = 900 x 900
```

__Finder__
<img src="./example2.png" width="270">

## Modifications ##

Rename `igen` to `igen.sh` and make your edits.

Pull requests are welcome.

## Requirements (inbuilt in macOS) ##

- [sips](https://ss64.com/osx/sips.html) - Scriptable Image Processing System
- [bc](https://www.gnu.org/software/bc/manual/html_mono/bc.html) - Basic Calculator 
- [sed](https://www.gnu.org/software/sed/manual/sed.html) - Stream Editor