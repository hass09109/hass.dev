<style type="text/css">
    :root {
  --primary: #ff3c00;          /* Fiery orange */
  --secondary: #b22222;        /* Dark red */
  --accent: #ffae00;           /* Amber/gold */
  --dark: #111111;             /* Deep charcoal black */
  --darker: #0a0a0a;           /* Almost true black */
  --text: #f0f0f0;             /* Light text for contrast */
}

body {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: 
        linear-gradient(135deg, rgba(17, 17, 17, 0.8), rgba(10, 10, 10, 0.8)),
        url('bos.jpg') no-repeat center center fixed;
      background-size: cover;
      color: var(--text);
      min-height: 100vh;
      overflow-x: hidden;
    }

#container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  position: relative;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  margin-bottom: 30px;
}

#clock, #date {
  font-weight: bold;
  font-size: 20px;
  color: var(--accent);
  background: rgba(0, 0, 0, 0.4);
  padding: 8px 15px;
  border-radius: 30px;
  box-shadow: 0 4px 15px rgba(255, 60, 0, 0.2);
}

.title-section {
  text-align: center;
  margin: 30px 0;
}

.title-section h1 {
  font-size: 28px;
  color: var(--primary);
  margin-bottom: 10px;
  text-shadow: 0 0 10px rgba(255, 60, 0, 0.3);
}

.title-section p {
  font-size: 16px;
  color: rgba(255, 255, 255, 0.6);
}

.buttons-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  margin: 40px 0;
}

.btn {
  background: linear-gradient(135deg, rgba(255, 60, 0, 0.15), rgba(178, 34, 34, 0.1));
  border: 1px solid rgba(255, 60, 0, 0.3);
  border-radius: 12px;
  padding: 20px;
  text-align: center;
  color: var(--text);
  font-size: 18px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  text-decoration: none;
  display: block;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(255, 60, 0, 0.4);
  background: linear-gradient(135deg, rgba(255, 60, 0, 0.25), rgba(178, 34, 34, 0.2));
  border-color: var(--primary);
}

.btn span {
  display: block;
  font-size: 14px;
  color: var(--accent);
  margin-top: 8px;
  font-weight: normal;
}

.footer {
  text-align: center;
  margin-top: 60px;
  padding: 30px 0;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.credits {
  font-size: 16px;
  color: rgba(255, 255, 255, 0.6);
}

.author {
  color: var(--accent);
  font-weight: bold;
  display: inline-block;
  margin-top: 10px;
  padding: 8px 20px;
  border-radius: 30px;
  background: rgba(255, 174, 0, 0.1);
  border: 1px solid rgba(255, 174, 0, 0.3);
}

.status-bar {
  background: rgba(0, 0, 0, 0.4);
  padding: 12px;
  border-radius: 8px;
  margin: 20px 0;
  text-align: center;
  font-size: 16px;
  color: var(--accent);
  min-height: 24px;
}

@keyframes pulse {
  0% { opacity: 0.6; }
  50% { opacity: 1; }
  100% { opacity: 0.6; }
}
