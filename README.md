# shake_plus

A flutter package to detect phone shakes.
Updated package using version `sensors_plus: ^6.1.0`.

To listen to phone shake:

    ShakeDetector detector = ShakeDetector.autoStart(
        onPhoneShake: () {
            // Do stuff on phone shake
        }
    );

OR

    ShakeDetector detector = ShakeDetector.waitForStart(
        onPhoneShake: () {
            // Do stuff on phone shake
        }
    );
    
    detector.startListening();

To stop listening:

    detector.stopListening();