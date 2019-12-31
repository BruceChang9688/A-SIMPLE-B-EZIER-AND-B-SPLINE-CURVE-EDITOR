Welcome to Project4!
This project is a simple Bezier and B-Spine curve editor.

*GLUI Prepare

Open glui-2.37 and make.
Open glui-2.37/bin and run example6.

*Initialize

Run example6 and input the file address.
I have make a file address for you. (test_curve.txt)
This original file contained three initial curves.
Two Bezier Curves. The first one is on the left bottom part. The second one is on the right bottom part.
One B-Spine Curve which is on the top of the screen.

Then we have a display window. A Bezier Curve interface Window. A B-Spine Curve interface Window. A save and quit command Window.

*Show curve

The display window is blank now. You can choose the checkbox for Bezier curve 1, Bezier curve 2 and B-Spine curve to display their curve(green), line segments(red) and control points respectively(blue, yellow for head and tail for purple). 

*For Bezier Curve operation in Bezier interface.

1.Move Points
You can move points in two Bezier curves by first pressing "MOVE POINTS" button and then press mouse to move the points you want.

2.Add Point to the tail
You can add points to each Bezier curves' tail by first pressing "ADD POINTS TO THE TAIL" and use mouse to point a new tail. Notice that the tale point is in color purple.

3.Add Point to the head
You can add points to each Bezier curves' head by first pressing "ADD POINTS TO THE HEAD" and use mouse to point a new head. Notice that the head point is in color yellow.

4.Delete Point
You can delete points in two Bezier curves by first pressing "DELETE POINT" and then click mouse to delete the point you want.

5.Insert Point
This operation is little different to other point operations. You can insert point by first pressing "INSERT POINT" and then use mouse to click on the point which you want to add follow with.(In this case you cannot insert points to the tail by clicking the present tail points, please use "Add points to the tail" operation.) Then the insert point will show up on the line segments follow by the points you click. Every time you want to insert a point you need to click on the "INSERT POINT" and repeat the operation above.

6.Resolution adjust
You can adjust each Bezier curve's resolution in 1 to 100.

*For B-Spine Curve operation in B-Spine interface.

For 1. Move Points, 2.Add points to the tail, 3.Add points to the head, 4.Delete Point, 5.Insert Point 6.Resolution adjust.
These operation is similar to Bezier Curve Operation.

7.Adjust number of order(k)
You can change the number of order(k) in 2 to the present number of control points.

8.Adjust knot value(Attention!)
You can adjust knot value by pressing button "ADJUST KNOT".
Then a new window for B-Spine-Knot-Adjust will shows up.

I have made all knots in 0 to 1.(normalized)
Here we have all normalized knots from u[1] to u[n+k-1].
For example, if we have 10 knots for this curve, here will be u[1],u[2],u[3],u[4],u[5],u[6],u[7],u[8]shows up.

You can adjust each knots position from the last knot position+0.01 to the next knot position-0.01.
For example, since the u[0] is locked on 0. So the u[1] can adjust from 0.01 to u[2]-0.01(this value is dynamic when you adjust u[2]).
Press "Close" to close this adjust window.

Notice that when you adjust knot on this window you cannot make other operation to the B-spine Curve.

*Save and Quit Window
1.Save all curves.
Whenever you want to save the curves, you can press "SAVE ALL" and all information for the curve would save in "Output_file.txt".
If you have save it once, press "SAVE ALL" would update the output file.

2.Quit
Press "QUIT" to quit the whole program.

*HAVE FUN*

By Dingheng (Bruce) Zhang
