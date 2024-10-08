## capacitor-timer-notification

A Capacitor plugin to create a timer notification that displays a countdown timer in the notification bar.

## Usage

Add the following to your `android/app/src/main/AndroidManifest.xml` file to declare the necessary permissions and service:

````xml
<uses-permission android:name="android.permission.FOREGROUND_SERVICE"/>
<uses-permission android:name="android.permission.FOREGROUND_SERVICE_MEDIA_PLAYBACK" />

<service
  android:name=".TimerService"
  android:enabled="true"
  android:exported="false"
  android:foregroundServiceType="mediaPlayback"/>




## Install

```bash
npm install capacitor-timer-notification
npx cap sync
````

## API

<docgen-index>

* [`startTimer(...)`](#starttimer)
* [`updateNotification(...)`](#updatenotification)
* [`stopTimer()`](#stoptimer)

</docgen-index>

<docgen-api>
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

### startTimer(...)

```typescript
startTimer(options: { duration: number; }) => Promise<void>
```

| Param         | Type                               |
| ------------- | ---------------------------------- |
| **`options`** | <code>{ duration: number; }</code> |

--------------------


### updateNotification(...)

```typescript
updateNotification(options: { duration: number; statusText: string; }) => Promise<void>
```

| Param         | Type                                                   |
| ------------- | ------------------------------------------------------ |
| **`options`** | <code>{ duration: number; statusText: string; }</code> |

--------------------


### stopTimer()

```typescript
stopTimer() => Promise<void>
```

--------------------

</docgen-api>
