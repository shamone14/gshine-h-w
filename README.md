
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>G-Shine Hardware</title>
<style>
:root {
  --bg: #f4f4f4;
  --text: #222;
  --accent: #2196f3;
  --input-bg: #fff;
  --cart-bg: #fff;
  --cart-text: #222;
}
body {
  font-family: Arial, sans-serif; margin: 0; background: var(--bg); color: var(--text);
  transition: background 0.3s, color 0.3s;
}
header {background: #333; color: white; text-align: center; padding: 0;}
header img {max-width: 100%; height: auto; display: block; margin: 0 auto;}
h1 {margin: 0; font-size: 2rem; padding: 0.5rem;}
.tagline {font-size: 1rem; font-style: italic; margin-bottom: 1rem;}
.search-container {
  position: sticky;
  top: 0;
  z-index: 100;
  background: var(--input-bg);
  text-align: center;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  padding: 1rem 0 0.5rem 0;
}
.search-container input {
  width: 80%;
  padding: 0.5rem;
  font-size: 1rem;
  border: 1px solid #bbb;
  border-radius: 6px;
  background: var(--input-bg);
  color: var(--text);
  transition: background 0.3s, color 0.3s;
}
.search-suggestions {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 80%;
  background: var(--input-bg);
  border: 1px solid #bbb;
  border-radius: 6px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  max-height: 180px;
  overflow-y: auto;
  text-align: left;
  margin-top: 2px;
  z-index: 9999;
  display: none;
  color: var(--text);
}
.search-suggestions li {
  padding: 8px 12px;
  cursor: pointer;
  border-bottom: 1px solid #f0f0f0;
  background: var(--input-bg);
}
.search-suggestions li:last-child {border-bottom: none;}
.search-suggestions li:hover {background: #f5faff;}
.category-filter-container {
  width: 100%;
  text-align: center;
  margin: 1em 0 0.5em 0;
