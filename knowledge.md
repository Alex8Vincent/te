# Git basics


- git add 'file' -> git add index.html
- git add . -> đưa toàn bộ thay đổi vào Stage Changes
- git commit -m'message' -> git commit -m'Add index.html and app .css'
- git push

# Branch

- branch 
- branch-name: feat/add-header, optimize-ui, quick-fix
- git checkout -b 'branch' -> git checkout -b optimize-ui
- Nếu chưa tồn tại dưới local thì ở giao diện Source Control sẽ có button là Publish Branch
- git push --set -upstream origin 'branch' -> git push --set-upstream origin optimize-ui
- create pull request
- merge code to branch Master
- git checkout 'branch' -> git checkout master -> chuyển sang nhánh khác
- git pull -> kéo code từ nhánh về
- git branch -D 'branch' -> git branch -D optimize-ui
# Rebase vs merge
# Conflict code
# Fetch vs pull

# Other
- git status: Kiểm tra trạng thái của các file
- ls: hiển thị danh sách các file và folder
- clear: clear teminal
- git log --oneline: cho xem mã hash có những lần commit trước
# Git reset

- Lệnh này dùng để reset lại các commit trước đó
- git reset --soft HEAD/hash_id: Lệnh này chỉ đơn giản là khi chúng ta quên add 1 file nào đó va chỉ muốn thêm vào sau khi reset
- git reset --mixed HEAD/hash_id: Lệnh này thì nó sẽ reset những commit trước đó và những staged changes
- git reset --hard HEAD/hash_id: Lệnh này rất nguy hiểm nên cần thận khi dùng nó sẽ xóa các commit trước đó (nếu có)

# Git Revert