import json

# 修正版 JSON（移除 refs/heads，改成 main）
fixed_data = {
    "ver": 1.0,
    "se": {
        "26": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/司馬昭.mp3"},
        "28": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/槓.mp3"},
        "30": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/吃.mp3"},
        "32": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/立直.mp3"},
        "34": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/哈哈胡.mp3"},
        "36": {"url": "https://raw.githubusercontent.com/JerryHaiya/jm/main/自摸.mp3"}
    }
}

# 輸出為 JSON 檔案
output_path = "/mnt/data/天鳳_fixed.json"
with open(output_path, "w", encoding="utf-8") as f:
    json.dump(fixed_data, f, ensure_ascii=False, indent=2)

output_path
