# Camera-Open-In-Android-Studio

#Runtime Camera Permission In Android Studio.

// Check Camera Permission already granted or not
        if (ContextCompat.checkSelfPermission(MainActivity.this, Manifest.permission.CAMERA) == PackageManager.PERMISSION_GRANTED) {
            Toast.makeText(MainActivity.this, "Camera permission is already granted", Toast.LENGTH_SHORT).show();
        } else {
            // Request Camera Permission
            ActivityCompat.requestPermissions(MainActivity.this, new String[]{Manifest.permission.CAMERA}, CAMERA_PERMISSION_REQUEST_CODE);
        }
