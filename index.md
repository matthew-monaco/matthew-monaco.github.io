---
layout: default
title: Home | Matthew Monaco
permalink: /
---

<style>
.popup {
  display: inline;
}

.popup input {
  display: none;
}

.popup label {
  cursor: pointer;
}

.popup-content {
  display: none;
  position: absolute;
  z-index: 1000;

  /* Center horizontally on the page */
  left: 50%;
  transform: translateX(-50%);

  width: min(600px, 90vw);
  padding: 10px;

  background: white;
  border: 1px solid #ccc;
  border-radius: 6px;
  box-shadow: 0 5px 25px rgba(0,0,0,0.25);
}

.popup input:checked + label + .popup-content {
  display: block;
}
</style>

<p id="bio-text">
I am a Paris-based composer and pianist, working across <span class="popup"><input type="checkbox" id="composition"><label for="composition"><strong><u>notated composition</u></strong></label><span class="popup-content"><iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//soundcloud.com/matthewtmonaco/thread-2025-for-ensemble"></iframe></span></span>, <span class="popup"><input type="checkbox" id="improvisation"><label for="improvisation"><strong><u>improvisation</u></strong></label><span class="popup-content"><iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//soundcloud.com/matthewtmonaco/thrum"></iframe></span></span>, and <span class="popup"><input type="checkbox" id="gamepieces"><label for="gamepieces"><strong><u>game pieces</u></strong></label><span class="popup-content"><iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//soundcloud.com/matthewtmonaco/rock-paper-scissors"></iframe></span></span>.
</p>

<script>
const bio = document.getElementById('bio-text');
const popups = document.querySelectorAll('.popup input');

function positionPopups() {
  const rect = bio.getBoundingClientRect();
  const top = rect.bottom + window.scrollY + 10;

  document.querySelectorAll('.popup-content').forEach(popup => {
    popup.style.top = top + 'px';
  });
}

popups.forEach(input => {
  input.addEventListener('change', () => {
    popups.forEach(other => {
      if (other !== input) {
        other.checked = false;
      }
    });

    positionPopups();
  });
});

window.addEventListener('resize', positionPopups);
window.addEventListener('scroll', positionPopups);

positionPopups();
</script>

<p>Feel free to contact me at <span style="color: green">matthew.t.monaco</span>[at]<span style="color: green">gmail</span>[dot]<span style="color: green">com</span>.</p>

<br>

<img src="IMG_9929_0.jpg" alt="Headshot" width="300">

<span class="green-bold">Upcoming events</span>

<p>8 Sep. - Performance of <strong>I've Heard That Song Before</strong> by Maria Eleonora Caminada at the <em>Festival Milano in Ascolto</em> (M<small>ILAN</small>, I<small>TALY</small>)</p>
<p>13 Sep. - Performance of <strong>I've Heard That Song Before</strong> by Maria Eleonora Caminada (F<small>UBINE</small> M<small>ONFERRATO</small>, I<small>TALY</small>)</p>
<p>19 Sep. -  Premiere of <strong>Zagzig</strong> by Ninon Hannecart-Ségal at the <em>Elisabeth Chojnacka Festival</em> (R<small>YBNA</small>, P<small>OLAND</small>)</p>
<p>20 Sep. - Performance of <strong>I've Heard That Song Before</strong> by Maria Eleonora Caminada (R<small>OZZANO</small>, I<small>TALY</small>)</p>
<p>20 Nov. - Premiere of a <strong>new work</strong> by the United Instruments of Lucilin at the <em>Rainy Days</em> festival (L<small>UXEMBOURG</small> C<small>ITY</small>, L<small>UXEMBOURG</small>)</p>
<p>25 Nov. - Premiere of <strong>Schmear</strong> for violoncello by Anna Grenzner as part of <em>Coincidence im Gespräch Vol.2</em> (G<small>RAZ</small>, A<small>USTRIA</small>)</p>

<br>
<span class="green-bold"><em>Past events (2026)</em></span>

<small><p>25 Jun. - Premiere of <strong>Rock Paper Scissors</strong> at <em>Bled Contemporary Music Week</em> (B<small>LED</small>, S<small>LOVENIA</small>)</p> 
<p>20 May - Premiere of <strong>I've Heard That Song Before</strong> by Maria Eleonora Caminada (M<small>ILAN</small>, I<small>TALY</small>)</p>
<p>15 Mar. - Performance of <strong>Scuffle</strong> by the Patsiaoura Ensemble <em>Reaching the Limits</em> festival (N<small>ICOSIA</small>, C<small>YPRUS</small>)</p>
<p>14 Mar. - Premiere of <strong>Scuffle</strong> by the Patsiaoura Ensemble at the <em>Reaching the Limits</em> festival (L<small>ARNACA</small>, C<small>YPRUS</small>)</p>
<p>7 Feb. - Duo performance with Myra Melford as part of the <em>CalPerformances</em> series (B<small>ERKELEY</small>, USA)</p></small>
