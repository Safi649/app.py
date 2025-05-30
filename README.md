import gradio as gr

def greet(message):
    if "who is your creator" in message.lower():
        return "I was created by Abbas Safi."
    return "Hello! Ask me anything."

iface = gr.Interface(fn=greet, inputs="text", outputs="text", title="Safi Chatbot")

iface.launch()
