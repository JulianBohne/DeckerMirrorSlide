# Mirror

<!-- Keyframe Plugin Setup -->
<script src="/julians-krams/keyframe-plugin/keyframeFragmentCreator.js"></script>
<script src="/julians-krams/keyframe-plugin/keyframe.js" type="module" defer></script>

<iframe id="mirror-explanation-page" src="/julians-krams/mirror/mirror-explanation.html" allowtransparency frameborder="0" style="border: none; width: 100%; height: 85%; position: absolute; left: 0; bottom: 0;"></iframe>
<script>
  Keyframes.setKeyframes('mirror-explanation-page', [
    { fixClipPlane: true, optimizeClipPlane: true },
    { overheadCam: true, showCameraFrustum: true },
    { showMirrorRay: true, fixClipPlane: false, optimizeClipPlane: false, instantClipPlane: true },
    { mirrorRayToMirrorCam: true },
    { showMirrorCameraFrustum: true },
    { showMirrorRay: false, mirrorRayToMirrorCam: false },
    { showRelativeCamPos: true, reflectionMathIndex: 0 },
    { showMirrorNormal: true, reflectionMathIndex: 1 },
    { projectRelativeCamPos: true, reflectionMathIndex: 2 },
    { subtractProjectedRelativeCamPos: true, reflectionMathIndex: 3 },
    { showReflectedVec: true, reflectionMathIndex: 4 },
    { reflectionMathIndex: 5 },
    { reflectionMathIndex: 6, showRelativeCamPos: false, showReflectedVec: false },
    { reflectionMathIndex: 7, showCameraForwardVector: true },
    { reflectionMathIndex: 8, showReflectedCameraForwardVector: true },
    { reflectionMathIndex: 9 },
    { reflectionMathIndex: 10, showReflectedCameraConstructedBasis: true },
    { reflectionMathIndex: 11, showReflectedCameraConstructedBasis: false, showCameraForwardVector: false, showMirrorNormal: false, showReflectedCameraForwardVector: false },
    { showCameraPreview: true, applyTextureToMirror: false },
    { flipCameraPreview: true },
    { applyTextureToMirror: true, fadeOutMirrorPreview: true },
    { moveCameraPreviewToBottom: true, frustumMathIndex: 0 },
    { frustumMathIndex: 1 },
    { frustumMathIndex: 2 },
    { frustumMathIndex: 3, showMirrorNormal: true, showMirrorCamDistanceToMirror: true },
    { frustumMathIndex: 4 },
    { frustumMathIndex: 5 },
    { frustumMathIndex: 6 },
    { frustumMathIndex: 7 },
    { frustumMathIndex: 8 },
    { frustumMathIndex: 9 },
    { fixClipPlane: true },
    { frustumMathIndex: 10 },
    { frustumMathIndex: 11 },
    { frustumMathIndex: 12 },
    { frustumMathIndex: 13, showInteractiveMath: true },
    { optimizeClipPlane: true },
    { fixClipPlane: false },
    { fixClipPlane: true },
    { frustumMathIndex: 14, showInteractiveMath: false, moveCameraPreviewToBottom: false, showMirrorNormal: false, showMirrorCamDistanceToMirror: false },
    { showCameraPreview: false, flipCameraPreview: false, overheadCam: false, showCameraFrustum: false, showMirrorCameraFrustum: false },
    { showWhatAboutVRAtIndex: 0 },
    { showWhatAboutVRAtIndex: 1 },
    { showWhatAboutVRAtIndex: 2 },
  ]);
</script>
