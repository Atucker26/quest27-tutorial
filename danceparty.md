# danceparty

## play music and show led

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString("Hello Lets dance!")
})
input.onButtonPressed(Button.B, function () {
    basic.showLeds(`
        . # . # .
        . . . . .
        # . . . #
        # # # # #
        . . . . .
        `)
})
input.onGesture(Gesture.Shake, function () {
    music.play(music.stringPlayable("C5 B A G E D C - ", 120), music.PlaybackMode.UntilDone)
})

