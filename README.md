- 👋 Hi, I’m @baekchoonghyun
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
baekchoonghyun/baekchoonghyun is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# 응답곡선 시각화
fig1, ax1 = plt.subplots()
ax1.plot(t, y)
ax1.set_xlabel('Time [s]')
ax1.set_ylabel('Amplitude')
ax1.set_title('Unit Step 응답곡선')
st.pyplot(fig1)

# 주파수 응답 보드선도 시각화
fig2, (ax2_mag, ax2_phase) = plt.subplots(2, 1)
ax2_mag.semilogx(w, mag)
ax2_mag.set_ylabel('Magnitude [dB]')
ax2_phase.semilogx(w, phase)
ax2_phase.set_xlabel('Frequency [rad/s]')
ax2_phase.set_ylabel('Phase [degrees]')
ax2_phase.set_title('주파수 응답 보드선도')
st.pyplot(fig2)
