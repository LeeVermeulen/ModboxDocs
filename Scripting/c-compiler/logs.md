---
title: "Logs"
slug: "logs"
hidden: false
createdAt: "2020-05-25T16:48:57.460Z"
updatedAt: "2020-05-26T15:46:02.648Z"
---
* Use Debug.Log / Debug.LogError / Debug.LogWarning for Engine errors. Errors that shouldn't happen regardless of player actions / what data they load. Engine Logs and Warnings only shown in LogUI if AllGameLogs is on. Errors are shown to the player just as 'Error Occured'
* MBLogs.LogUser / MBLogs.LogUserError / MBLogs.LogUserWarning are for User actions. LogUserError should be used when trying to use a Method in MBScript in the wrong way / don't have permission for. All 'User Logs' are shown in the Log UI in game.
* There is also LogSavedData / LogNetData, for log/warning/errors - for logging issues with data from online / saved.