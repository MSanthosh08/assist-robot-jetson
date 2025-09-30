# Assist-robot-jetson

This repository is a **submodule** of the master project  
[**intelligent-assistive-robot**](https://github.com/Msanthosh08/intelligent-assistive-robot).  
It contains all code and files for the jetson_nano

## ⚡ Tasks & Responsibilities

This module handles the **high-level computation and integration platform**.

- Install and configure the **Jetson Nano** OS environment with ROS/ROS2.
- Implement the **navigation stack**:
  - SLAM mapping (e.g., GMapping or RTAB-Map).
  - Localization (AMCL).
  - Path planning (move_base or Nav2).
- Integrate LiDAR (RPLIDAR A1) and odometry data from hardware for real-time map updates.
- Create a communication bridge between Jetson Nano and Arduino:
  - Send velocity commands.
  - Receive sensor feedback.
- Manage **system startup scripts**, package dependencies, and deployment instructions.
- Provide APIs for Vision and Voice modules to send/receive navigation data.


---

## 🔑 Access Through the Main Repository
If you already cloned the master repo, you do **not** need to clone this module separately.

1. Clone the master project with all submodules  
   ```bash
   git clone --recurse-submodules git@github.com:Msanthosh08/intelligent-assistive-robot.git
   cd intelligent-assistive-robot 
2. Enter this module folder
   ```bash
   cd jetson_nano   # e.g., cd hardware (jetson_nano or Vision, or voice-nlp)

3. Work only inside this folder.
You have write access here but read-only access to other modules.
## 💡 Daily Workflow
---------------------------------------------------------------------------------------------------

| Action              | Command                              | Notes                          |
| ------------------- | ------------------------------------ | ------------------------------ |
| Check status        | `git status`                         | Shows modified/untracked files |
| Pull latest changes | `git pull`                           | Always do this first           |
| Stage files         | `git add <file>` or `git add .`      | Stage specific or all files    |
| Commit changes      | `git commit -m "Meaningful message"` | Short, clear commit message    |
| Push to GitHub      | `git push`                           | Upload your commits            |
| Create branch       | `git checkout -b feature/<name>`     | For new features               |
| Switch branch       | `git checkout <branch>`              | Return to `main` when done     |

###### ⚠️ Always run git pull before committing to avoid conflicts.
----------------------------------------------------------------------------------------------------
🔄 Updating the Master Pointer.

1. After you push changes here, the integration lead will update the master repo:
   ```bash
    cd ../..
    git add <module-folder>
    git commit -m "Update <module-name> submodule to latest"
    git push
# or
# ⚙️ Standalone Clone

1. You can also work on this module directly:
   ```bash
   git clone git@github.com:MSanthosh08/assist-robot-jetson_nano.git
   cd assist-robot-jetson_nano
2. 📧 Contact

For access issues or merge conflicts, contact Santhosh M 
- Mobile: 7418499308
- Mail: m.santhosh0804@gmail.com